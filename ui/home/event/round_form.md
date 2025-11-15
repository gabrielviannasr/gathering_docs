# 🔄 Round Form Page

Tela acessada via: **Home Page (Eventos) → Event List (Adicionar / Editar) → Event Form (Rodadas) → Round List (Adicionar / Editar) → Round Form**

Formulário para gerenciar uma rodada do evento.

## ✏️ Campos

- **Formato** (`format_name`) — select
- **Vencedor** (`id_player_winner`)  
  - Definido apenas pelo botão **Definir Vencedor**
  - Campo bloqueado para edição direta

---

## Lista de Jogadores (Pesquisa)

### 🔎 Filtros
- Nome (LIKE %name%)

### 📑 Colunas
- Nome (name)

### ✔️ Funcionalidades
- Botão "Adicionar Jogador"
- Lista carregada automaticamente
- Paginação

## Lista de Jogadores (Score)

Jogadores já adicionados à rodada.

### 📑 Colunas
- Nome
- Indicador de vencedor (se aplicável)

### ✔️ Funcionalidades
- Botão "Remover Jogador" (por item)
- Botão "Definir Vencedor" (por item)

---

## ✔️ Funcionalidades

- Botão “Cancelar”
- Botão “Salvar”
  - Atualizar campos automaticamente:
    - Jogadores (players)
    - Premiação (prize)
    - Pote dos Derrotados (loser_pot)
