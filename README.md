# deployments-manual 🚀

🚀 Simple instructions on how to deploy a static web application to popular hosting platforms.

All examples assume your app is built into the `dist/` directory. If your build tool
uses a different output directory (e.g. `build/`, `public/`), adjust the paths.

## Table of contents 📖

- [Netlify](#netlify-)
- [Vercel](#vercel-)
- [Cloudflare Pages](#cloudflare-pages-)
- [Surge.sh](#surgesh-)
- [Railway](#railway-)

## Netlify 🌊

Option 1 — drag & drop (no terminal needed):

1. Build your app: `npm run build`
2. Go to <https://app.netlify.com/drop>
3. Drag the `dist/` directory onto the page — done, you get a public URL

Option 2 — CLI:

1. Install the CLI: `npm install --global netlify-cli`
2. Log in: `netlify login`
3. Build your app: `npm run build`
4. Deploy: `netlify deploy --prod --dir=dist`

Docs: <https://docs.netlify.com/cli/get-started/>

## Vercel ▲

1. Install the CLI: `npm install --global vercel`
2. Log in: `vercel login`
3. Run in the project directory: `vercel --prod`
4. Answer a few questions (defaults are fine) — you get a public URL

Docs: <https://vercel.com/docs/cli>

## Cloudflare Pages ☁️

1. Install the CLI: `npm install --global wrangler`
2. Log in: `wrangler login`
3. Build your app: `npm run build`
4. Deploy: `wrangler pages deploy dist/`

Docs: <https://developers.cloudflare.com/pages/get-started/direct-upload/>

## Surge.sh ⚡

The fastest option — no account setup needed up front:

1. Build your app: `npm run build`
2. Deploy: `npx surge dist/`
3. On the first run, type your email and password to create a free account

Docs: <https://surge.sh/help/getting-started-with-surge>

## Railway 🚂

Best suited for full-stack apps (backend + database), but it can serve static sites too:

1. Install the CLI: `npm install --global @railway/cli`
2. Log in: `railway login`
3. Create a project: `railway init`
4. Deploy: `railway up`

Docs: <https://docs.railway.com/guides/cli>

## License 📄

[The MIT License](https://piecioshka.mit-license.org) @ 2026
