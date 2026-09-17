# Wavvy

Monorepo skeleton for cross-border payments with Next.js frontend and separate Node/Fastify backend.

## Workspaces

- `frontend/` — Next.js app, Privy auth, Monad client setup, payment UI area
- `backend/` — Fastify API, Privy verification, Monad server wallet/RPC, Nansen, Agora payment services

## Setup

```bash
npm install
cp frontend/.env.example frontend/.env.local
cp backend/.env.example backend/.env
npm run dev
```

## Provider setup

- Privy: add `NEXT_PUBLIC_PRIVY_APP_ID`, `PRIVY_APP_ID`, `PRIVY_APP_SECRET`
- Monad: confirm chain ID/RPC, add backend signing key only if server-side transactions needed
- Nansen: add API key/base URL in backend env
- Agora: add API key/base URL/webhook secret/settlement account in backend env

No application code added yet; only project structure, workspace config, dependencies, and env templates.
