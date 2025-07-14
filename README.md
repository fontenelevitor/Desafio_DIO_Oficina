# 📌 Projeto: Esquema Conceitual - Oficina Mecânica

Este repositório apresenta o modelo conceitual (diagrama ER) para um sistema de controle e gerenciamento de ordens de serviço em uma **oficina mecânica**. A modelagem foi desenvolvida com base em uma narrativa-problema fornecida no contexto de um desafio prático de modelagem de banco de dados.

## 📖 Contexto da Narrativa

Clientes levam seus veículos até a oficina para consertos ou revisões periódicas. Cada veículo é designado a uma equipe de mecânicos, que avalia os problemas, preenche a OS (Ordem de Serviço), consulta os valores dos serviços com base em uma tabela de mão de obra e inclui também os valores das peças utilizadas. O cliente então autoriza a execução dos serviços. A mesma equipe é responsável por executar os serviços até a data de entrega.

## 🎯 Objetivo

Criar um modelo conceitual representando todas as entidades, relacionamentos e atributos necessários para o gerenciamento completo de ordens de serviço da oficina.

## 🔍 Principais Entidades

- **Cliente:** armazena dados dos clientes.
- **Veículo:** dados sobre veículos trazidos pelos clientes.
- **Ordem de Serviço (OS):** representa o serviço solicitado.
- **Equipe:** grupo de mecânicos responsável pela OS.
- **Mecânico:** dados dos profissionais da oficina.
- **Serviço:** serviços realizados na OS, com valor de mão de obra.
- **Peça:** peças utilizadas nos consertos, com preço.
- **Item_Peca:** liga OS às peças utilizadas com quantidade.

## 📘 Assunções

- Cada veículo pertence a apenas um cliente.
- Cada OS está vinculada a um único veículo e a uma equipe.
- Cada OS pode conter vários serviços e várias peças.
- Uma peça pode ser utilizada em várias OS.
- Os valores de OS são compostos por soma dos serviços e das peças.
