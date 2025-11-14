# 📱 Estrutura Inicial do Aplicativo — Gathering App

*(Mobile First + Web Responsivo)*

Este documento descreve o layout inicial, navegação e principais componentes da interface do aplicativo Gathering.

---

## 🧭 Menu Inferior (Bottom Navigation)

O menu inferior será fixo em todas as páginas principais.
Ícones sugeridos (Lucide, Ionicons, Material Symbols).

| Aba                             | Ícone            | Função                                              |
| ------------------------------- | ---------------- | --------------------------------------------------- |
| **Home**                        | `home`           | Tela inicial com atalhos para as principais funções |
| **Extrato**                     | `arrows-up-down` | Histórico de transações e movimentações             |
| **Carteira**                    | `wallet`         | Saldo do jogador + ações de saque/deposito          |
| **Relatórios** ou **Dashboard** | `graph`          | Indicadores, ranking e estatísticas                 |

---

## 🏠 Home Page (Tela Inicial)

A **Home** é a tela principal do aplicativo, responsável por apresentar rapidamente:

1. **A confra atualmente selecionada**
2. **O menu de navegação por cards**

O layout segue o conceito **mobile-first**, garantindo boa responsividade para iOS, Android e web.

---

## 🎗️ Banner superior — Confra Selecionada

Na parte superior haverá um **banner** destacando a confra ativa.
Este banner ajuda o usuário a perceber em qual “contexto” está trabalhando.

### ✔️ Regras:

* **Título** — Exibe o **nome da confra** em destaque.
* **Subtítulo** — Abaixo, exibe o **ano da confra**.
* Caso nenhuma confra esteja selecionada:
  * Nome: **"Selecione uma confra"**
  * Ano: **"-"**

### ✔️ Layout (visual esperado)

```
[ =============================== ]
[            DIRETORIA            ]
[              2025               ]
[ =============================== ]
```

ou, sem confra:

```
[ =============================== ]
[      Selecione uma confra       ]
[               -                 ]
[ =============================== ]
```

### ✔️ Espaçamento

* **Espaçamento acima e abaixo** do banner para separá-lo claramente do menu.
* Fonte do nome maior que a do ano.

---

## 🧱 Menu da Home — Grid 2×N (Cards)

A Home exibe um **grid de cards**, com 2 cards por linha.
Cada card é uma ação principal do app.

### ✔️ Regras gerais dos cards

* 2 cards por linha (mobile)
* Espaçamento consistente entre cards (vertical e horizontal)
* Cards quadrados, bordas levemente arredondadas
* O conteúdo de cada card terá **3 linhas**:
  1. **Ícone**
  2. **Título** em *negrito*, sem ícone ao lado
  3. **Subtítulo** — descrição curta

---

## 📌 Lista de Cards do Menu

| # | Ícone    | Título        | Subtítulo     | Função                                   |
| - | -------- | ------------- | ------------- | ---------------------------------------- |
| 1 | reunion  | **Confras**   | Gerenciar     | CRUD de gatherings                       |
| 2 | calendar | **Eventos**   | Gerenciar     | CRUD de eventos                          |
| 3 | trophy   | **Rank**      | Classificação | Ranking consolidado da confra            |
| 4 | people   | **Jogadores** | Gerenciar     | CRUD de players                          |
| 5 | cards    | **Formatos**  | Modos de jogo | CRUD de formatos                         |
| 6 | list     | **Regras**    | Como funciona | Explicação da lógica e regras do sistema |

### Observação sobre o ícone *Formatos*

Para “modos de jogo”, sugestões:

* `layers`
* `cards`
* `dice`
* `shapes`

---

## ✔️ Observação de Implementação (para o futuro frontend)

O banner superior deve ser **interativo**:

* Ao tocar no nome/ano → abrir seleção de confra.
* Quando uma confra for alterada, toda a Home deve atualizar seu contexto.

---

## 🏠 Home Page

A página inicial será composta por um banner informando a confra selecionada com o ano abaixo, e por um menu composto por **cards** distribuídos em **grid 2×N**, no estilo mobile-first com responsividade automática para desktop.

### ✔️ Regras de layout do menu:

* 2 cards por linha (mobile)
* Espaçamento vertical e horizontal constante
* Cards quadrados, bordas levemente arredondadas
* O conteúdo de cada card terá **3 linhas**:
  1. **Ícone**
  2. **Título** (sem ícone ao lado) — *negrito*
  3. **Subtítulo** — descrição curta

---

## 📄 Extrato (Histórico de Transações)

### Conteúdo:

* Lista cronológica de transações
* Cada item contendo:
  * Jogador
  * Data
  * Ícone do tipo (`deposit`, `withdraw`, `result`, `entry`)
  * Valor (R$)
  * Descrição (opcional)

* Filtros:
  * Por jogador
  * Por tipo (depósito, saque, inscrição, resultado)
  * Por período

---

## 💰 Carteira

### Conteúdo:

* Lista dos jogadores em ordem alfabética
* Cada item contendo:
  * Jogador
  * Saldo (R$)
* Botões:
  * “Depositar”
  * “Sacar”

---

## 📊 Relatórios / Dashboard

Tela dedicada a estatísticas e métricas gerais.

### Indicadores possíveis:

* Winrate
* Desempenho por formato
* Resumo da gathering (events, rounds confra_pot, loser_pot, prize)
* Posições no ranking (por gathering)
* Gráficos (pizza, barras, linha do tempo)
