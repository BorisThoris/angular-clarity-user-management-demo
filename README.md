# User Hub Admin

A legacy Angular 9 portfolio demo for a small user-management workflow built with VMware Clarity UI. The app demonstrates Angular routing, reusable form components, localStorage-backed CRUD state, and Clarity-styled screens.

## What it shows

- Angular module/routing structure.
- VMware Clarity UI components.
- Local user creation, editing, viewing, and deletion.
- Parent/child component communication with `@Input` and `@Output`.
- Basic image fallback handling for user avatars.
- GitHub Pages-ready static build output.

## Tech stack

- Angular 9
- TypeScript
- VMware Clarity
- RxJS

## Run locally

```bash
npm install
npm start
```

Open `http://localhost:4200`.

This demo stores its user-management state in `localStorage`; no backend is required. The npm scripts set the legacy OpenSSL provider flag needed by Angular/Webpack on modern Node versions.

## Verify

```bash
npm run build
```

## Legacy note

This is an older demo project that has been preserved and reframed as a personal portfolio sample. It is not intended to represent a current production stack.

## Cloudflare Pages

- Pages project name: `user-hub-admin`
- GitHub repository: `BorisThoris/user-hub-admin`
- Production branch: `master`
- Root directory: `.`
- Build command: `NODE_OPTIONS=--openssl-legacy-provider npx ng build`
- Build output directory: `dist/Demo`
- Public URL target: `https://user-hub-admin.pages.dev/`

Do not enable Cloudflare Access for the demo deployment. Leave frame-blocking headers unset so the portfolio can iframe the public build.
