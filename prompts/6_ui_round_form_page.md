# 🟦 **ROUND FORM PAGE**

### Card eo Evento

- Reutilizar componente

Mockup:

const event = ref({
idFormat: 2,
format: { id: 1, name: 'Conquest' },
date: '2025-01-20',
players: 8,
rounds: 8
})

---

### Card do Round

Duas colunas (label / valor):

* Rodada
	- Circulo gradiente
	- justify-between
* **Vencedor** (Nome / Sem vencedor)
	- Destaque fundo verde / negrito
	- Não editável, apenas pelo botão definir vencedor
* **Status** (Ativa / Cancelada)
* Toogle Button (Ativar / Cancelar)
  	- Label on left and bold

Mockup: { id: 1, round: 1, idPlayerWinner: 5, players: 6, prize: 45.00, loserPot: 15.00 }

---

### Card da Configuração das Taxas

Duas colunas (label / valor):

* Título: Configuração das Taxas
* Jogadores
* Premiação
* Pote dos Derrotados

Mockup:
{ id: 1, players: 6, prize: 45.00, loserPot: 15.00 }

---

### Card dos Filtros

Título: Filtros

- filtro de busca de jogador por nome em toda a base
- Ação de adicionar jogador a lista

---

### Lista de Jogadores

- Permitir selecionar jogador para poder definir vencedor com o botão "definir jogador"
- Nome
- Ícone vencedor
	- Troféu Amarelo / 32px
	- justify-between
- Botão remover (por item)

Mockup: [
{ id: 1, name: 'Anderson Dias' },
{ id: 2, name: 'Arthur Leal' },
{ id: 3, name: 'Cindomar Ferreira' },
{ id: 4, name: 'Gabriel Vianna' },
{ id: 5, name: 'Jean Benevides' },
{ id: 6, name: 'Jhonny Dias' }
]


### Botões

* Botão "Definir Vencedor"
	- Linha única e em destaque
	- Ícone troféu branco
* Botão cancelar
* Botão salvar (mesmo gradiente padrão utilizado)
