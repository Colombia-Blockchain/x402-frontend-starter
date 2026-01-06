# Cronos x402 Agentic Treasury - Frontend

Frontend for the autonomous payment system on Cronos testnet. Users create payment "intents" with conditions that an AI agent can execute when conditions are met.

## Tech Stack

- Next.js 14 (App Router)
- TypeScript
- Tailwind CSS
- wagmi/viem
- RainbowKit
- TanStack Query

## Getting Started

### Prerequisites

- Node.js 18+
- pnpm

### Installation

```bash
pnpm install
```

### Environment Setup

Copy `ENV_EXAMPLE` to `.env.local`:

```bash
cp ENV_EXAMPLE .env.local
```

Configure the following variables:

| Variable | Description | Default |
|----------|-------------|---------|
| `NEXT_PUBLIC_API_URL` | Backend API URL | `http://localhost:3001` |
| `NEXT_PUBLIC_WALLET_CONNECT_PROJECT_ID` | WalletConnect project ID | - |
| `NEXT_PUBLIC_CHAIN_ID` | Chain ID | `338` (Cronos testnet) |

### Development

```bash
pnpm dev
```

### Build

```bash
pnpm build
pnpm start
```

### Lint

```bash
pnpm lint
```

## Project Structure

```
src/
├── app/                 # Next.js App Router pages
│   ├── page.tsx         # Landing page
│   └── dashboard/       # Treasury management
├── components/          # React components
├── hooks/               # React Query hooks
├── services/            # API service layer
└── styles/              # Global styles
```

## License

MIT
