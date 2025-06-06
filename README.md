# A3_BancoDados_SQL_
## Modelagem de Banco de Dados (ER) e SQL no DB Fiddle
###  Diagrama ER:

![WhatsApp Image 2025-06-05 at 22 41 16](https://github.com/user-attachments/assets/10ddfa73-6060-4b38-a83d-571809b600a7)

## Link do DB Fiddle: https://www.db-fiddle.com/f/7DHyYa4Dzvc9fbN22ahVi5/0

## 📘 Significado das Tabelas e Colunas

### 🧑 `Usuario`
Armazena dados dos usuários do sistema.
- `usuario_id`: Identificador único (chave primária)
- `nome`: Nome completo do usuário
- `email`: E-mail do usuário (único)
- `criado_em`: Data/hora de criação automática do cadastro

---

### 💼 `Carteira`
Representa uma carteira de criptomoedas vinculada a um usuário.
- `carteira_id`: Identificador único da carteira (PK)
- `usuario_id`: Referência ao usuário dono da carteira (FK)
- `nome`: Nome da carteira (ex: "Carteira Pessoal")
- `saldo`: Saldo atual da carteira (valor em moeda local)
- `criado_em`: Data/hora de criação da carteira

---

### 🪙 `Criptomoeda`
Contém as criptomoedas disponíveis para negociação.
- `cripto_id`: Identificador único (PK)
- `nome`: Nome completo da criptomoeda
- `simbolo`: Símbolo (ex: BTC, ETH) — valor único

---

### 📈 `Transacao`
Registro de cada transação de compra de criptomoeda.
- `transacao_id`: Identificador da transação (PK)
- `carteira_id`: Carteira que realizou a transação (FK)
- `cripto_id`: Criptomoeda envolvida (FK)
- `quantidade`: Quantidade de criptomoeda adquirida
- `valor_total`: Valor da transação em moeda local
- `data_transacao`: Data/hora da transação!

  
## Exemplo de resultado das consultas: 
![EXEMPLOS](https://github.com/user-attachments/assets/fc8b3ec4-4077-4d1f-914b-6babe25a1114)

![exemplo2](https://github.com/user-attachments/assets/0c2325ac-4d73-4e7e-aadd-869905ff2812)
![exemplo 3](https://github.com/user-attachments/assets/71605ea4-ebb7-4a38-afac-bedfdca2cd44)




## 👥 Participantes

Este projeto foi desenvolvido por:

- **Ana Julia Cota Brum**
- **Leonardo Oliveira Morais**


