# Scriptline — Setup Guide

The fastest path is one click. Everything below is there if you want it,
not because you need it.

## The one-click way (recommended — no terminal, no zip)

1. Open this link: **https://github.com/teamglowhaus/scriptline**
2. Click the purple **"Deploy with Vercel"** button near the top of that page
3. Sign in to Vercel (free — email only, no card)
4. When asked for `ANTHROPIC_API_KEY` and `PEXELS_API_KEY`, paste them in
   (see "Getting your API keys" below if you don't have them yet)
5. Click **Deploy** — about a minute later your live app opens automatically

Done. You don't need anything else on this page.

## Getting your API keys

**Anthropic API key** — writes your content:
1. [platform.claude.com](https://platform.claude.com) → sign in
2. **API Keys** → **Create Key** → copy it (starts with `sk-ant-`)
3. **Billing** → add $5 credit (required separately from a Claude subscription — a few cents per generation)

**Pexels API key** — finds background images, free:
1. [pexels.com/api](https://www.pexels.com/api/) → sign up → copy your key

## If you'd rather use a terminal

```bash
git clone https://github.com/teamglowhaus/scriptline.git
cd scriptline
npm install
npx vercel login
npx vercel
npx vercel env add ANTHROPIC_API_KEY production
npx vercel env add PEXELS_API_KEY production
npx vercel --prod
```

## If something goes wrong

**Generation fails with a credit or billing error** — your Anthropic account needs API credit added separately from any Claude subscription. Go to `platform.claude.com → Billing` and add funds.

**Images never load** — double check your Pexels key has no extra spaces.

**I changed something — how do I update my live site?** — commit your change and push; Vercel redeploys automatically if you used the one-click method (it connects to your own GitHub copy).

---

See [LICENSE.md](./LICENSE.md) for usage terms.
