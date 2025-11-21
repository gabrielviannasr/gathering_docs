# ✅ **PROMPT PROFISSIONAL — Telas: Rank, Extrato e Regras Globais**

> **Instrução geral:**
> **Não recrie layouts que já existem.**
> **Ajuste somente as telas indicadas, mantendo o estilo visual atual:** cores, gradientes, cartões, ícones outline (MDI/Feather), espaçamentos e hierarquia visual já aplicados nas telas anteriores.

---

# 🏆 **GERAR / AJUSTAR A TELA: RANK PAGE**

**Acesso:** Home Page → Rank → Rank Page

### **Header**

* Título: **"Rank"**
* Subtítulo: **"{ANO} – {NOME DA CONFRA}"**

  * Ex.: “2025 – DIRETORIA”
* Mostrar o **formato** em texto, logo abaixo, não editável.
  Ex.: “Formato: Conquest”

### **Lista de jogadores (em cards ou list rows)**

Cada linha deve exibir:

* Rank (posição) — número grande, à esquerda
* Nome do jogador
* Vitórias
* Rodadas
* Ícone de seta “>” para detalhes (mesmo estilo da lista de eventos)

**Importante:** manter compacto, mas extremamente leitura fácil.

# 🏆 **GERAR / AJUSTAR A TELA: RANK DETAIL**

**Acesso:** Home Page → Rank → Rank Page → Rank Detail

Exibir em 2 colunas (nome da coluna e valor):
* Rank
   * Esta coluna represnta posição — exibir um número grande no valor
* Nome do jogador
* Vitórias
* Rodadas
* Positivo (R$)
* Negativo (R$)
* Saldo Rankeado
* Pote dos Derrotados (R$)
* Saldo Final (R$)

---

Mockup para usar nas telas Rank e Rank Detail:

| Rank | Jogador | Vitórias | Rodadas | Positivo | Negativo | Saldo Rankeado | Pote dos Derrotados | Saldo Final |
|1 |Tobias Souza |2 |4 |90,00 |40,00 | 50,00| 0,00| 50,00|
|2 |Jhonny Dias |2 |6 |90,00 |60,00 | 30,00| 0,00| 30,00|
|3 |Arthur Leal |1 |5 |45,00 |50,00 | -5,00| 0,00| -5,00|
|4 |Valmir Vicente |1 |6 |45,00 |60,00 |-15,00| 0,00|-15,00|
|5 |Anderson Dias |1 |7 |45,00 |70,00 |-25,00| 0,00|-25,00|
|6 |Jean Benevides |1 |8 |45,00 |80,00 |-35,00| 0,00|-35,00|
|7 |Cindomar Ferreira |0 |6 | 0,00 |60,00 |-60,00|60,00|  0,00|
|7 |Gabriel Vianna |0 |6 | 0,00 |60,00 |-60,00|60,00|  0,00|

---

# 💸 **GERAR / AJUSTAR A TELA: EXTRATO (HISTÓRICO DE TRANSAÇÕES)**

**Substituir o topo atual (que está como “Transactions”) por:**

### **Header**

* Título grande: **“Extrato”**
* Subtítulo menor: **“Histórico de Transações”**
* Subtítulo menor: **“{ANO} – {NOME DA CONFRA}”**
* Ícone de filtros permanece, mesmo estilo atual

### **Filtros**

* Jogador (select)
* Tipo (select: Depósito, Saque, Inscrição, Resultado)
* Mês (select)

  * Opções: **"Todos" + Janeiro … Dezembro** (em ordem correta)

### **Cards da lista de transações (estilo atual da UI)**

Cada item contém:

* Ícone e tipo de transação (nesta ordem, primeiro o ícone):

  * **Depósito:** seta para cima
  * **Saque:** seta para baixo
  * **Inscrição:** ícone de ticket/cash/entry
  * **Resultado:** troféu/estrela
* Nome do jogador
* Valor (positivo/negativo)
* Data
* Descrição
* Indicação “>” para detalhes (mesmo padrão da lista de eventos)

### **Bottom Navigation Bar**

* Home
* Extrato (ativo)
* Carteira
* Relatórios

---

# 📌 **REGRAS GLOBAIS IMPORTANTES — APLICAR EM TODAS AS NOVAS TELAS**

## 🟥 **1. A Bottom Navigation Bar aparece APENAS nestas telas:**

* **Home** — ícone: `home`
* **Extrato** — ícone: `arrows-up-down` (substituir o atual na tela de extrato)
* **Carteira** — ícone: `wallet`
* **Relatórios** — ícone: `graph`

➡️ **Nenhuma outra tela deve exibir a bottom bar.**
Isso inclui: Confras, Jogadores, Formatos, Eventos, Rank, Rounds, Forms etc.

---

## 🟦 **2. Telas de listas precisam permitir abrir o formulário pelo card**

Aplicar nas telas:

* Confras List
* Jogadores List
* Formatos List
* Eventos List (já faz isso, manter)

Sempre usando seta “>” à direita.

---

## 🟩 **3. Na tela de lista de eventos, exibir o ícone do tipo de formato**

Exemplo:

* Commander → carta
* Conquest → carta
* Tiny Leaders → carta
* Outras categorias → ícone correspondente ao tipo

---

## 🟧 **4. Ajuste na lista de configurações de taxas do Event Form**

Onde hoje aparece:

* Jogadores
* Pote Derrotados
* Pote Confra

**Substituir por:**

* Jogadores
* Premiação
* Pote da Confra

Manter o estilo das linhas já existentes no design atual.

Adicionar botão **“Remover configuração”** em cada linha (ícone lixeira discreto).

---

## 🟪 **5. Na Home Page, o botão “Selecionar Confra” deve abrir opções:**

* Diretoria 2025
* Diretoria 2024
* Diretoria 2023

Pode ser:

* Modal
* Side sheet
* Dropdown estilizado

Escolher a opção mais coerente com o design atual.

---

# 🔵 **Opcional: Referência de ícones (Material Design Icons – Outline)**

Sugira ao editor figma:

* Confras: `mdi-account-group` **(3+ pessoas)**
* Eventos: `mdi-calendar-month`
* Rank: `mdi-trophy-outline`
* Jogadores: `mdi-account-multiple`
* Formatos (cartas): `mdi-cards-playing-outline`
* Regras: `mdi-format-list-bulleted`
* Extrato: `mdi-arrow-up-down`
* Dashboards/Relatórios: `mdi-chart-line`
* Carteira: `mdi-wallet-outline`

---

# ✨ **FRASE FINAL DO PROMPT (crucial para IA de design)**

> “Keep the existing aesthetic exactly as is — gradients, colors, spacing, icon style. Only apply the described updates. Do NOT redesign from scratch. Produce high-fidelity mockups following the current UI system.”
