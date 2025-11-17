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
* Ano

### **Botões**

* Cancelar
* Salvar

---

# 📝 **GERAR A TELA: EVENT FORM PAGE**

Tela acessada via: **Home Page → Eventos → Event List (Adicionar/Editar) → Event Form**

---

### **Campos**

* **Formato (select)**
  Opções:

  * Adedonha ou Stop
  * Commander
  * Conquest
  * Detetive
  * Ludo
  * Tiny Leaders

* **Taxa da Confra**

* **Taxa da Rodada**

---

### **💰 Lista de Configurações (Taxas por Jogadores)**

Abaixo do formulário principal, exibir uma lista dinâmica no formato **card por linha**, contendo:

* Jogadores (número)
* Premiação
* Pote dos Derrotados
* **Botão "Remover"** (por card)

### **Botões relacionados**

* **Adicionar Configuração** (adiciona novo card à lista)

---

### **Botões finais da tela**

* Cancelar
* Salvar
* **Gerenciar Rodadas** → redireciona para Round List Page
  *(não cria rodadas diretamente)*

---

### **Botões**

* Cancelar
* Salvar
* **Gerenciar Rodadas** → redireciona para Round List Page
  *(não cria rodadas diretamente)*

---

# 🔄 **GERAR A TELA: ROUND LIST PAGE**

Tela acessada via:
**Home Page → Eventos → Event List (Editar) → Event Form → Gerenciar Rodadas → Round List**

### **Colunas do Card**

* Data/hora
* Nº da Rodada
* Formato
* Cancelada? (SIM/NÃO)
* Jogadores
* Premiação
* Pote dos Derrotados

### **Botões**

* Adicionar Rodada
* Editar (por item)
* Score (por item)
* Cancelar/Restaurar Rodada (por item)

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

