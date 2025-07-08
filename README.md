# caencore.com

This is a minimal [Astro](https://astro.build/) site configured for deployment on [Cloudflare Pages](https://pages.cloudflare.com/).

## Local development

Install dependencies and start the dev server:

```bash
npm install
npm run dev
```

## Building

To create a production build, run:

```bash
npm run build
```

The output will be generated in the `dist/` folder.

## Running with Cloudflare Workers

Build for server-side rendering and preview locally using Wrangler:

```bash
npm run build
npm run preview
```

This serves your built site using Cloudflare Workers so you can test SSR locally.

## Deployment

Deploy with Cloudflare Pages using either the Git integration or the Wrangler CLI.

### Git deployment

1. Push your code to a Git repo (e.g., GitHub).
2. In the Cloudflare dashboard, create a **Pages** project and connect your repo.
3. Use the **Astro** framework preset, set the build command to `npm run build`,
   and `dist` as the output directory.
4. Save and deploy.

### CLI deployment

Install Wrangler and run the deploy script:

```bash
npm run deploy
```
