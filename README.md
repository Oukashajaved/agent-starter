# AI Chat Agent — Cloudflare Workers

A production-ready AI chat agent built on Cloudflare's Agents SDK.

## What it does
- **Tool-use** — server-side auto-execute, client-side browser tools, and human-in-the-loop approval tools
- **Scheduling** — one-time, delayed, and recurring (cron) task execution
- **Voice / Vision** — image input with vision-capable model support
- **MCP integration** — connects to external MCP servers for extended tool libraries
- **WebSocket persistence** — real-time streaming with automatic reconnection and message persistence

## Stack
- Cloudflare Workers + Agents SDK
- React 19 + Tailwind CSS v4
- Vite 8 + Wrangler 4
- TypeScript 6
- AI SDK (Vercel) — model-agnostic, swap to OpenAI/Anthropic/Workers AI

## Run locally
```bash
npm install
npm run dev
```
Open `http://localhost:5173`

## Deploy
```bash
npm run deploy
```
Live on Cloudflare's global edge network instantly.

## Try it
- *"What's the weather in Miami?"* — server-side tool
- *"What timezone am I in?"* — client-side browser tool  
- *"Calculate 9999 * 8888"* — approval tool (asks before running)
- *"Remind me in 10 minutes to check email"* — scheduling
- Drop an image → *"What's in this?"* — vision
