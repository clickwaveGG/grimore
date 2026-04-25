# Grimore

> Transforme um PDF em um Grimório.

SaaS de Q&A em PDF para universitários — sobe qualquer livro, apostila ou atividade e converse com ele.

## Estrutura

- `app/` — Landing page (V1.0, HTML estático)
- `brand/` — Brand assets, paleta, logos pixel art, preview do brandbook

## Stack planejada (V1.0)

- Next.js 15 + Tailwind + shadcn
- Supabase (auth + Postgres + pgvector + storage)
- Anthropic Haiku 4.5 (LLM com prompt caching)
- OpenAI text-embedding-3-small (embeddings)
- Asaas (Pix recorrente + cartão)
- Vercel (deploy)

## Rodar local

Não exige build. Servidor estático qualquer:

```bash
cd app
npx serve
```

Abre `http://localhost:3000`.

## Deploy

Auto-deploy via Vercel a cada push na `main`.
