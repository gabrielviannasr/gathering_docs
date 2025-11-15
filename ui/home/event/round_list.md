# 🔄 Round List Page

Tela acessada via: **Home Page (Eventos) → Event List (Adicionar / Editar) → Event Form (Rodadas) → Round List**

Lista todas as rodadas configuradas para o evento.

## 📑 Colunas

| Campo | Descrição |
|-------|-----------|
| Data/hora | createdAt |
| N° da Rodada | round |
| Formato | format_name |
| Cancelada | SIM / NÃO |
| Jogadores | players |
| Premiação | prize |
| Pote dos Derrotados | loser_pot |

## ✔️ Funcionalidades
- Botão "Score" (por item)
- Botão “Cancelar / Restaurar Rodada” (por item)
- Botão “Adicionar Rodada”
- Botão “Editar” (por item)
- Lista carregada automaticamente
- Paginação

---

## ✔️ Regras importantes

- O número da rodada (**round**) é gerado automaticamente pelo backend.
- Rodadas são listadas sempre em ordem crescente (1 → N)
- Uma rodada cancelada não afeta cálculos de premiação do evento
