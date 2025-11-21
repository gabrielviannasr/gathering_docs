# 🔄 **GERAR A TELA: RANK LIST PAGE**

Tela acessada via:
**Home Page → Rank → Rank Event List → Rank List**

### **Card do Formato do Evento**

  * Ícone do formato ao lado esquerdo.
    * Forma: Círculo
    * Fundo gradiente
  * Formato / Sem formato
  * Data do evento
  * X jogadores - Y rodadas

  Mockup: { 
    id: 2, 
    idFormat: 2,
    format: { id: 2, name: 'Conquest' , type: { id: 1, name: 'Cartas' } }, 
    date: '2025-01-21',
    players: 8, 
    rounds: 8
  },

### **Bloco de filtros**

  * Botão Adicionar Rodada

### **Colunas do Card**

* Nº do Rank
* **Jogador** (destaque)
* Ícone de troféu - X vitórias - Y rodadas
* A seta ">"

Mockup Result: [
{ idEvent: 1, idPlayer: 7, rank: 1, wins: 2, rounds: 4, positive: 90.00, negative: 40.00, rankBalance:  50.00, loserPot:  0.00, finalBalance:  50.00 },
{ idEvent: 1, idPlayer: 6, rank: 2, wins: 2, rounds: 6, positive: 90.00, negative: 60.00, rankBalance:  30.00, loserPot:  0.00, finalBalance:  30.00 },
{ idEvent: 1, idPlayer: 2, rank: 3, wins: 1, rounds: 5, positive: 45.00, negative: 50.00, rankBalance:  -5.00, loserPot:  0.00, finalBalance:  -5.00 },
{ idEvent: 1, idPlayer: 8, rank: 4, wins: 1, rounds: 6, positive: 45.00, negative: 60.00, rankBalance: -15.00, loserPot:  0.00, finalBalance: -15.00 },
{ idEvent: 1, idPlayer: 1, rank: 5, wins: 1, rounds: 7, positive: 45.00, negative: 70.00, rankBalance: -25.00, loserPot:  0.00, finalBalance: -25.00 },
{ idEvent: 1, idPlayer: 5, rank: 6, wins: 1, rounds: 8, positive: 45.00, negative: 80.00, rankBalance: -35.00, loserPot:  0.00, finalBalance: -35.00 },
{ idEvent: 1, idPlayer: 3, rank: 7, wins: 0, rounds: 6, positive:  0.00, negative: 60.00, rankBalance: -60.00, loserPot: 60.00, finalBalance:   0.00 },
{ idEvent: 1, idPlayer: 4, rank: 7, wins: 0, rounds: 6, positive:  0.00, negative: 60.00, rankBalance: -60.00, loserPot: 60.00, finalBalance:   0.00 }
]

### **Regras**

* Paginação