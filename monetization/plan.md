# 💰 Plano de Monetização — Gathering

O Gathering terá um modelo híbrido de monetização:

---

## 🆓 Plano Gratuito (Free)
- Limite de 1 confra ativa
- Limite de 4 eventos por mês
- Limite de 6 jogadores por evento
- Limite de 6 rodadas por evento
- Dashboard básico (saldo + histórico)
- Anúncios discretos

---

## ⭐ Plano Premium
- Gatherings ilimitadas
- Eventos ilimitados
- Jogadores ilimitados
- Rodadas ilimitadas
- Dashboard avançado (rank completo, histórico detalhado, estatísticas)
- Sem anúncios

---

## 🎯 Estratégia de Monetização
- Público-alvo: grupos recorrentes de TCG (Commander), boardgames, RPG, mesas mensais etc.
- Modelo de preço simples: R$ 14,90 / mês (faixa estimada: R$ 9,90 – R$ 19,90)
- Teste gratuito de 30 dias
- Possibilidade futura de plano anual com desconto

---

## 💻 Funcionalidades Necessárias (Backend + App)

Para habilitar o sistema de planos:

### Backend
  - Criar tabela subscription_plan
  - Criar tabela user_subscription
  - Regras de rate limit sobre entidades (confras, eventos, jogadores…)
  - Middleware/Interceptor de verificação de plano
  - Endpoint para upgrade/downgrade de plano
  - Integração com meio de pagamento (Mercado Pago, Stripe, IAP, Google Play Billing…)

### App (Frontend)
  - Tela de criação de conta
  - Tela de login (e opção “esqueci minha senha”)
  - Tela explicativa dos planos
  - Tela de upgrade (checkout)
  - Indicação visual de limites quando o usuário estiver no plano Free
