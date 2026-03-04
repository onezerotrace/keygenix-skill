# Keygenix Keys — Project Keys Record

> ⚠️ This file is a template. Replace placeholders with your own generated keys.
> Private keys must NEVER be stored here — use `.env` or a secrets manager.

## Generated: YYYY-MM-DD

### API Auth Key (for authenticating all API calls)
- **Public Key:** `<YOUR_API_AUTH_PUBLIC_KEY_HEX>`
- **Register on:** keygenix.pro dashboard → API Keys section

### AuthKey (for authorizing sign/export operations)
- **Public Key:** `<YOUR_AUTH_PUBLIC_KEY_HEX>`
- **Use as:** `authPubKey` parameter when creating/importing keys via API

## How to Generate

```bash
node client.js keygen   # Run twice — once for API Auth Key, once for AuthKey
```

Copy the `publicKey` values into this file. Store `privateKey` values in `.env` only.

## Setup Steps

1. Register at https://keygenix.pro
2. Create an organization → note down `orgCode`
3. Create a wallet → note down `walletCode`
4. Register API Auth Public Key in dashboard
5. Copy `.env.example` to `.env`, fill in private keys + org/wallet codes
6. Test: `node client.js list-keys`
