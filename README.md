# Wavvy

Monorepo skeleton for cross-border payments with Next.js frontend and separate Node/Fastify backend.

## Workspaces

- `frontend/` — Next.js app, Monad client setup, payment UI area
- `backend/` — Fastify API, Monad RPC, Nansen, Agora payment services

## Setup

```bash
npm install
cp frontend/.env.example frontend/.env.local
cp backend/.env.example backend/.env
npm run dev
```

## Provider setup

- Monad: confirm chain ID/RPC
- Nansen: add API key/base URL in backend env
- Agora: add API key/base URL/webhook secret/settlement account in backend env

No application code added yet; only project structure, workspace config, dependencies, and env templates.
