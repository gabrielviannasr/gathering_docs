# 🟦 **RANK DETAIL PAGE**

**Acesso:** Home → Rank → Rank Event List → Rank Page → Rank Detail

### Card Evento

- Reutilizar card

### Card Rank

Duas colunas (label / valor):

* Jogador
* Rank (número grande / destaque)
    - Cicrulo gradiente
	- 1º lugar: Icon medalha de ouro
	- 2º lugar: Icon medalha de prata
	- 3º lugar: Icon medalha de bronze
	
* Vitórias
    - Cicrulo cinza
* Rodadas
    - Cicrulo cinza
* Positivo (R$)
	- Verde
* Negativo (R$)
	- Vermelho
* Saldo Rankeado (R$)
* Pote dos Derrotados (R$)
* Saldo Final (R$)
	- Roxo
	- Número grande (destaque)

Mockup:
  const event = ref({
    idFormat: 2,
    format: { id: 1, name: 'Conquest' },
    date: '2025-01-20',
    players: 8,
    rounds: 8
  })

  const player = ref({
    id: 7,
    name: 'Tobias Souza'
  })

  const rank = ref({
    idEvent: 1,
    idPlayer: 7,
    rank: 1,
    wins: 2,
    rounds: 4,
    positive: 90.0,
    negative: 40.0,
    rankBalance: 50.0,
    loserPot: 0.0,
    finalBalance: 50.0
  })
