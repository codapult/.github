# Codapult

**The modular Next.js SaaS boilerplate with auth, payments, teams, admin, AI, and infrastructure already wired together.**

Auth, billing, teams, admin panel, AI layer, SSO, and infrastructure work as one system out of the box. Start lean with only the modules your MVP needs, then scale without rebuilding the foundation.

---

### What's included

| Category           | Modules                                                              |
| ------------------ | -------------------------------------------------------------------- |
| **Auth**           | Email/password, OAuth, magic links, TOTP 2FA, SAML SSO, SCIM         |
| **Billing**        | Stripe, LemonSqueezy, Polar — switchable via env var                 |
| **Teams**          | Organizations, RBAC, invitations, seat billing, audit log            |
| **Admin**          | User management, feature flags, webhooks, A/B testing, metrics       |
| **AI**             | Streaming chat, RAG pipeline, embeddings, quotas, OpenAI + Anthropic |
| **Infrastructure** | Docker, Terraform, Pulumi, Helm chart, GitHub Actions CI/CD          |
| **API**            | tRPC v11, REST, optional GraphQL, type-safe end-to-end               |

70+ modules. Each independently removable via CLI. No dead code.

---

### Architecture

Codapult is built around the adapter pattern — auth, payments, storage, jobs, embeddings, and notifications each sit behind a unified interface. Swap providers by changing one environment variable. No rewrites.

```
AUTH_PROVIDER=kinde             # better-auth | kinde
PAYMENT_PROVIDER=lemonsqueezy   # stripe | lemonsqueezy | polar
STORAGE_PROVIDER=r2             # local | s3 | r2
JOB_PROVIDER=bullmq             # memory | bullmq
```

---

### Stack

![Next.js](https://img.shields.io/badge/Next.js-black?style=flat-square&logo=next.js)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Turso](https://img.shields.io/badge/Turso-4FF8D2?style=flat-square&logo=turso&logoColor=black)
![Drizzle](https://img.shields.io/badge/Drizzle-C5F74F?style=flat-square&logo=drizzle&logoColor=black)
![tRPC](https://img.shields.io/badge/tRPC_v11-2596BE?style=flat-square&logo=trpc&logoColor=white)
![Stripe](https://img.shields.io/badge/Stripe-635BFF?style=flat-square&logo=stripe&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-black?style=flat-square&logo=vercel)

---

### Quick start

```bash
npx create-codapult my-app
```

The interactive wizard configures auth, payments, and storage in under 5 minutes.

---

**[Website](https://codapult.dev)** · **[Live Demo](https://demo.codapult.dev)** · **[Docs](https://codapult.dev/docs)** · **[Pricing](https://codapult.dev/#pricing)**
