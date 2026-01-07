# YouTube Ninja Analytics

## Estrutura do Projeto

<details>
<summary><strong>youtube-ninja-analytics/</strong> (clica para expandir a raiz do projeto)</summary>

- <details>
  <summary><strong>frontend/</strong></summary>

  - <details open>
    <summary><strong>src/</strong></summary>

    - <details>
      <summary><strong>app/</strong></summary>

      - bootstrap/ # Providers consolidados
      - layouts/ # Layouts principais
      - router/ # Rotas e guards
      - App.jsx

    </details>

    - <details open>
      <summary><strong>domains/</strong> ← DOMÍNIOS PRINCIPAIS (DDD)</summary>

      - <details>
        <summary><strong>auth/</strong></summary>

        - ui/
        - application/
        - infrastructure/
        - pages/
        - types/

      </details>

      - onboarding/
      - dashboard/

      - <details>
        <summary><strong>youtube/</strong> # Consolidado com subdomínios</summary>

        - channels/
        - videos/
        - analytics/

      </details>

      - seo/
      - keywords/
      - competitors/
      - ai/
      - content-calendar/
      - audience/

      - <details>
        <summary><strong>reports/</strong> ← Domínio que queres destacar</summary>
      </details>

      - billing/ # Faturação completa
      - team/
      - automation/
      - notifications/
      - settings/

    </details>

    - <details>
      <summary><strong>shared/</strong> # Componentes, hooks, utils reutilizáveis</summary>

      - ui/ # Buttons, cards, tables, charts...
      - hooks/
      - services/
      - utils/

    </details>

    - locales/ # i18n por domínio
    - assets/
    - <details>
      <summary><strong>public/</strong> # Landing pages públicas</summary>
    </details>
    - tests/
    - main.jsx

  </details>

  - public/
  - package.json

</details>

- <details>
  <summary><strong>backend/</strong></summary>

  - <details open>
    <summary><strong>src/</strong></summary>

    - core/ # Config, middleware, utils globais

    - <details>
      <summary><strong>domains/</strong> # Mesmos domínios do frontend</summary>

      - auth/
      - users/
      - youtube/
      - billing/ # Stripe, planos, invoices
      - reports/
      - ... (outros 12 domínios)

    </details>

    - infrastructure/ # DB, cache, queue, jobs, webhooks
    - api/v1/
    - bootstrap/

  </details>

  - prisma/

</details>

- shared/ # Tipos e utils compartilhados front/back
- infra/ # Docker, Kubernetes, Terraform
- docs/ # Documentação completa
- .github/
- package.json
- docker-compose.yml

</details>

> **Nota**: Esta árvore é totalmente interativa no GitHub, GitLab, Bitbucket e na maioria dos visualizadores de Markdown modernos. Cada pasta pode ser expandida/colapsada individualmente.
