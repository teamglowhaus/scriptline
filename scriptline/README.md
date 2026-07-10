# Scriptline

An AI content generator for UGC scripts, Instagram, TikTok, and digital
product promo content — writes in a real, human voice, finds matching
background images, and builds upload-ready graphics.

## 🚀 Deploy in one click (recommended)

No terminal, no zip file, no coding. Click the button, sign in, paste two
API keys, done.

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fteamglowhaus%2Fscriptline&env=ANTHROPIC_API_KEY,PEXELS_API_KEY&envDescription=API%20keys%20needed%20to%20run%20Scriptline%20%E2%80%94%20see%20the%20link%20below%20for%20where%20to%20get%20them&envLink=https%3A%2F%2Fgithub.com%2Fteamglowhaus%2Fscriptline%23getting-your-api-keys&project-name=scriptline&repository-name=scriptline)

**What happens when you click it:**
1. Vercel asks you to sign in (or create a free account — just email, no card needed)
2. It copies this project into your own account automatically
3. It asks you to paste in two API keys (see below for where to get them)
4. Click **Deploy** — about a minute later, your live app opens automatically

That's the whole process. Skip everything below unless you want it.

## Getting your API keys

You need two, both required for the deploy screen above.

**Anthropic API key** (writes your content):
1. Go to [platform.claude.com](https://platform.claude.com) → sign in
2. **API Keys** (left sidebar) → **Create Key** → copy it (starts with `sk-ant-`)
3. **Billing** (left sidebar) → add $5 credit — required separately from any Claude subscription, billed per generation (a few cents each)

**Pexels API key** (finds background images, completely free):
1. Go to [pexels.com/api](https://www.pexels.com/api/) → sign up → copy your key

## What it does

- **4 creator modes**: UGC Video Creator, Instagram Creator, TikTok Creator, Digital Product Promo
- Writes hooks, captions, and full scripts in a real, human voice — never sounds like AI
- Auto-finds 3 matching background images for every post via Pexels
- Builds upload-ready graphics (feed posts, carousels, stories) with your text overlaid — click download, post it
- Mobile-friendly, dark mode, fully responsive

## Prefer the terminal instead?

If you'd rather deploy from the command line:

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

See [SETUP-GUIDE.md](./SETUP-GUIDE.md) for the fully spelled-out, beginner
version of this path.

## License

See [LICENSE.md](./LICENSE.md) for usage terms — personal and commercial
use is welcome; reselling the raw source code is not.
