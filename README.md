# Estrutura do Projeto YouTube Ninja Analytics

<details>
<summary><strong>Clique para expandir a árvore completa do projeto</strong> (colapsável)</summary>

```tree
youtube-ninja-analytics/
├── frontend/
│   ├── src/
│   │   ├── app/
│   │   │   ├── bootstrap/              # Providers consolidados
│   │   │   ├── layouts/                # Layouts principais
│   │   │   ├── router/                 # Rotas e guards
│   │   │   └── App.jsx
│   │   ├── domains/                    # ← DOMÍNIOS PRINCIPAIS (DDD)
│   │   │   ├── auth/
│   │   │   │   ├── ui/
│   │   │   │   ├── application/
│   │   │   │   ├── infrastructure/
│   │   │   │   ├── pages/
│   │   │   │   └── types/
│   │   │   ├── onboarding/
│   │   │   ├── dashboard/
│   │   │   ├── youtube/                # Consolidado com subdomínios
│   │   │   │   ├── channels/
│   │   │   │   ├── videos/
│   │   │   │   └── analytics/
│   │   │   ├── seo/
│   │   │   ├── keywords/
│   │   │   ├── competitors/
│   │   │   ├── ai/
│   │   │   ├── content-calendar/
│   │   │   ├── audience/
│   │   │   ├── reports/                # ← Domínio que você quer destacar
│   │   │   ├── billing/                # Faturação completa
│   │   │   ├── team/
│   │   │   ├── automation/
│   │   │   ├── notifications/
│   │   │   └── settings/
│   │   ├── shared/                     # Componentes, hooks, utils reutilizáveis
│   │   │   ├── ui/                     # Buttons, cards, tables, charts...
│   │   │   ├── hooks/
│   │   │   ├── services/
│   │   │   └── utils/
│   │   ├── locales/                    # i18n por domínio
│   │   ├── assets/
│   │   ├── public/                     # Landing pages públicas
│   │   ├── tests/
│   │   └── main.jsx
│   ├── public/
│   └── package.json
│
├── backend/
│   ├── src/
│   │   ├── core/                       # Config, middleware, utils globais
│   │   ├── domains/                    # Mesmos domínios do frontend
│   │   │   ├── auth/
│   │   │   ├── users/
│   │   │   ├── youtube/
│   │   │   ├── billing/                # Stripe, planos, invoices
│   │   │   ├── reports/
│   │   │   └── ... (outros 12 domínios)
│   │   ├── infrastructure/             # DB, cache, queue, jobs, webhooks
│   │   ├── api/v1/
│   │   └── bootstrap/
│   └── prisma/
│
├── shared/                             # Tipos e utils compartilhados front/back
├── infra/                              # Docker, Kubernetes, Terraform
├── docs/                               # Documentação completa
├── .github/
├── package.json
└── docker-compose.yml
