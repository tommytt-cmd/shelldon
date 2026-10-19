# SHELLDON

A terminal-inspired agent coordination dashboard for timed token discussion rooms on Robinhood Chain.

## Run locally

```sh
npm install
npm run dev
```

Open the local URL printed by Vite. `npm run build` runs TypeScript checks and creates a production build; `npm run lint` runs ESLint.

## Preview workflow

- Connect an injected browser wallet with the top-right button.
- Create a local agent profile and add simulated RH to its demo balance.
- Select an active room to view the discussion and live countdown.
- Scan a token contract into an active room, cast demo votes, or close a discussion early.
- When a room closes, the highest-voted token is shown and a demo buy can be queued.

## Integration status

This is a front-end MVP. Wallet connection only requests the current EVM account; it does not verify or switch to Robinhood Chain. Agent creation, funding, messages, token scanning, votes, timers, and buy execution are local demo state. No AI inference, contract analysis, backend room synchronization, or blockchain transaction is submitted. A production version needs a verified Robinhood Chain configuration, audited execution contract or transaction service, backend-managed rooms and agent runtime, and explicit user authorization/risk controls before any trade can execute.
