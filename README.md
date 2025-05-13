 Sistema de Adoção de Pets – MongoDB Atlas

Este projeto faz parte da disciplina de Banco de Dados II, e representa a modelagem e estruturação de um sistema de adoção de pets, utilizando um banco de dados não-relacional (MongoDB) hospedado na plataforma MongoDB Atlas.

 Estrutura do Repositório

Este repositório contém os seguintes arquivos:

- `pets_exemplo_completo.json`  
  Contém 9 pets com dados reais de teste (espécie, raça, porte, saúde, etc.)

- `adotantes_exemplo_completo.json`  
  Contém 4 adotantes, com dados pessoais e vínculo com pets adotados.

- `compatibilidade_completo_atualizado.json`  
  Avaliações de compatibilidade entre adotantes e pets com critérios, pontuação e status.

- `historico_rastreabilidade_completo.json`  
  Registro do resgate de todos os pets, incluindo local, data, tempo e responsável.

- `esquema_mongodb_adocao_pets.pdf`  
  Diagrama visual explicando a estrutura e relacionamento entre as coleções.

---

 Como importar no MongoDB Atlas

1. Crie um cluster no MongoDB Atlas.
2. Acesse a aba **Collections** do seu banco.
3. Crie as coleções com os seguintes nomes:
   - `pets`
   - `adotantes`
   - `compatibilidade`
   - `historico_rastreabilidade`
4. Em cada coleção, clique em **"Import"** → **"Import JSON"** e selecione o arquivo correspondente.

---

 Exemplos de Consultas MongoDB

Pets disponíveis para adoção

{ "status": "disponível para adoção" }

---
Histórico de um pet específico

{ "pet_id": ObjectId("68221570aec72754a1c4e724") }

---

Compatibilidade entre adotante e pets

{ "adotante_id": ObjectId("607c7f0f8d4c4a5eb5fbd1fa") }

---

 Regras de Compatibilidade
As comparações entre adotante e pet consideram:

Espécie, porte, sexo

Condições de saúde

Compatibilidade social

Fatores impeditivos (por exemplo, pets que não convivem bem com outros)

A pontuação é somada por categoria e define o status: "Aprovado" ou "Rejeitado".

---

Nome: Eduardo Martins Emidio
Data:13/05/2025
Matéria: Banco de Dadod II
