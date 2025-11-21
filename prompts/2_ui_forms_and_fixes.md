# ✅ **PROMPT PROFISSIONAL — GERAR TELAS DE FORMULÁRIO (Forms) PARA O APP GATHERING**

*(com regras de navegação incluídas)*

Use este prompt para gerar **todas as telas de formulário** do app, seguindo o design atual do Figma e mantendo a estética existente.

---

# 🎨 **ESTILO GERAL (MANTER)**

* Mesmo gradiente, cores, sombras e spacing das telas anteriores
* Componentes modernos (Material 3 + iOS 17)
* Textos bem hierarquizados
* Cards minimalistas e ícones outline
* Layout mobile-first, responsivo
* **⚠️ IMPORTANTE:** *Não recriar UI do zero — ajustar mantendo o que já existe*

---

# 🧭 **REGRA GLOBAL DE NAVEGAÇÃO (IMPORTANTE)**

### **❌ NÃO exibir a Bottom Navigation Bar em Forms e Listas internas**

A bottom bar só existe nas 4 telas principais:

* Home
* Extrato
* Carteira
* Relatórios

### **✔️ Listas internas e Forms NÃO devem ter barra inferior.**

Exemplos:
Gathering List, Event List, Player List, Format List, Event Form, Round List, Round Form etc.

---

# 📝 **GERAR A TELA: PLAYER FORM PAGE**

Tela acessada via: **Home Page → Jogadores → Player List (Adicionar/Editar) → Player Form**

### **Campos**

* Nome (input text)

### **Botões**

* Cancelar
* Salvar

---

# 📝 **GERAR A TELA: FORMAT FORM PAGE**

Tela acessada via: **Home Page → Formatos → Format List (Adicionar/Editar) → Format Form**

### **Campos**

* Nome
* Pontos de Vida
* Tipo do Jogo (select):
  * Cartas
  * Eletrônicos
  * Imaginação
  * Papel e Caneta
  * Tabuleiro

### **Botões**

* Cancelar
* Salvar

---

# 📝 **GERAR A TELA: GATHERING FORM PAGE**

Tela acessada via: **Home Page → Confras → Gathering List (Adicionar/Editar) → Gathering Form**

### **Campos**

* Nome

### **Botões**

* Cancelar
* Salvar

---

# 📝 **GERAR A TELA: EVENT FORM PAGE**

Tela acessada via: **Home Page → Eventos → Event List (Adicionar/Editar) → Event Form**

---

* Título do card: Evento

### **Campos (Card)**

* **Formato (select)**
  Opções:
  * Commander
  * Conquest
  * Tiny Leaders

* **Taxa da Confra**

* **Taxa da Rodada**

Mockup: { id: 1, idFormat: 1 (Commader), confraFee: 20.0, RoundFee: 10.0 }
ou
Mockup: { id: 1, format: { id: 1, name: "Commader" }, confraFee: 20.0, RoundFee: 10.0 }

---

### **💰 Lista de Configurações (Taxas por Jogadores)**

Abaixo do formulário principal, exibir uma lista dinâmica no formato **card por linha**, contendo:

* Jogadores (número)
* Premiação
* Pote dos Derrotados
* **Botão "Remover"** (por card)

Mockup: [
  { id: 1, players: 5, prize: 40.0, loserPot: 10.0 },
  { id: 1, players: 6, prize: 45.0, loserPot: 15.0 }
]


### **Botões relacionados**

* **Adicionar Configuração** (adiciona novo card à lista)

---

### **Botões finais da tela**

* Cancelar
* Salvar

---

### **Botões**

* Cancelar
* Salvar

---

# 🔄 **GERAR A TELA: ROUND LIST PAGE**

Tela acessada via:
**Home Page → Round → Round Event List → Round List**

### **Card do Formato do Evento**

  * Ícone do formato ao lado esquerdo.
    * Forma: Círculo
    * Fundo gradiente
  * Formato
  * Data do evento
  * X jogadores - Y rodadas

  Mockup: { 
    id: 2, 
    format: { id: 2, name: 'Conquest' , type: { id: 1, name: 'Cartas' } }, 
    date: '2025-01-21',
    players: 8, 
    rounds: 8
  },

### **Bloco de filtros**

  * Botão Adicionar Rodada

### **Colunas do Card**

* Nº da Rodada
* Formato - X jogadores
* **Vencedor**
* Badge de status (Ativa / Cancelada)
* A seta ">"

Mockup Rounds: [
  { idPlayerWinner: 5, round: 1, players: 6, prize: 45.00, loserPot: 15.00, canceled: false },
  { idPlayerWinner: 7, round: 2, players: 6, prize: 45.00, loserPot: 15.00, canceled: false },
  { idPlayerWinner: 8, round: 3, players: 6, prize: 45.00, loserPot: 15.00, canceled: false },
  { idPlayerWinner: 1, round: 4, players: 6, prize: 45.00, loserPot: 15.00, canceled: false },
  { idPlayerWinner: 7, round: 5, players: 6, prize: 45.00, loserPot: 15.00, canceled: false },
  { idPlayerWinner: 6, round: 6, players: 6, prize: 45.00, loserPot: 15.00, canceled: false },
  { idPlayerWinner: 2, round: 7, players: 6, prize: 45.00, loserPot: 15.00, canceled: false },
  { idPlayerWinner: 6, round: 8, players: 6, prize: 45.00, loserPot: 15.00, canceled: false }
]

Mockup Players: [
  { id: 1, name: 'Anderson Dias' },
  { id: 2, name: 'Arthur Leal' },
  { id: 3, name: 'Cindomar Ferreira' },
  { id: 4, name: 'Gabriel Vianna' },
  { id: 5, name: 'Jean Benevides' },
  { id: 6, name: 'Jhonny Dias' },
  { id: 7, name: 'Tobias Souza' },
  { id: 8, name: 'Valmir Vicente' },
]

### **Regras**

* Rodadas sempre por ordem crescente
* Round gerado automaticamente
* Paginação se necessário

---

# 🔄 **GERAR A TELA: ROUND FORM PAGE**

Tela acessada via:
**Home Page → Eventos → Event List (Editar) → Event Form → Round List → Round Form**

### **Campos**

* Formato (select)
* Vencedor (bloqueado — selecionado via botão)

---

### **Lista de Jogadores (Pesquisa)**

* Filtro: Nome
* Lista com botão **Adicionar Jogador**
* Paginação

---

### **Lista de Jogadores (Score)**

* Nome
* Indicador de vencedor
* Botão Definir Vencedor
* Botão Remover

---

### **Botões**

* Cancelar
* Salvar

  * Atualiza automaticamente:

    * Jogadores
    * Premiação
    * Pote dos Derrotados

---

# 📌 FRASE FINAL (para AIs de design)

> “Generate only the screens requested, in high-fidelity UI, maintaining the current visual identity, spacing, color gradients, icons, typography and components already established. Do not redesign from scratch — only extend and adapt the existing UI.”

