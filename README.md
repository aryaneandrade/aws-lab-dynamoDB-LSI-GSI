# 🔍 Laboratório Prático: Amazon DynamoDB com LSI e GSI

Este laboratório foi desenvolvido como parte da formação na **Escola da Nuvem** e tem como foco a **modelagem de dados NoSQL** utilizando **Amazon DynamoDB**, com ênfase em **índices secundários locais (LSI)** e **globais (GSI)** para otimização de consultas.

---

## 📌 Objetivo

Demonstrar na prática como criar uma tabela no DynamoDB com chave composta e configurar índices secundários para consultas eficientes, explorando a escalabilidade e flexibilidade da modelagem NoSQL.

---

## 🧱 Componentes Utilizados

- **Amazon DynamoDB** – Banco de dados NoSQL gerenciado
- **CloudShell e Console da AWS** – Para criação e consultas
- **Comando `batch-write-item`** – Para inserção de dados em lote
- **Índices Secundários**:  
  - **LSI (Local Secondary Index)** – Consultas por `Status`  
  - **GSI (Global Secondary Index)** – Consultas por `Status` e `ValorTotal`

---

## ⚙️ Atividades Realizadas

- Criação de tabela com chave composta: `UserID` (partition key) + `DataPedido` (sort key)
- Implementação de LSI para habilitar consultas por `Status` mantendo a mesma partition key
- Implementação de GSI para consultas por `Status` + `ValorTotal`, permitindo maior flexibilidade
- Inserção de dados usando `batch-write-item` via CloudShell
- Execução de queries com 100% de eficiência com base em índices

---

## 🧪 Resultados Esperados

- Consultas eficientes por atributos não indexados na tabela original
- Flexibilidade na leitura de dados com diferentes padrões de acesso
- Prática consolidada de modelagem orientada a acesso com DynamoDB

---

## 🖼️ Exemplos Visuais

> Substitua por capturas de tela reais no repositório:

- Criação da tabela com LSI configurado  
  ![LSI](./imagens/criacao-lsi.png)

- Configuração de GSI na mesma tabela  
  ![GSI](./imagens/criacao-gsi.png)

- Consulta com eficiência 100% (uso de índice)  
  ![Query Efficiency](./imagens/query-sucesso.png)

---

## 🔒 Licença

Este projeto é de uso educacional, sem fins comerciais.
