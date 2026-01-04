# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.

---

## Deployment (Vercel) ⚙️

To deploy on Vercel reliably:

- Ensure the **Build Command** is `npm run build` (or leave default). We added a `vercel-build` script which runs `npm run build`.
- Ensure the **Output Directory** is `dist` (this is Vite's default). The included `vercel.json` explicitly sets this.

Environment variables (recommended):

- `VITE_EMAILJS_USER` — your EmailJS user ID
- `VITE_EMAILJS_SERVICE` — your EmailJS service ID
- `VITE_EMAILJS_TEMPLATE` — your EmailJS template ID

Set these in the Vercel dashboard under Project Settings → Environment Variables. Locally, you can create a `.env` file with `VITE_` prefixed variables (do NOT commit secrets to git).

These changes help avoid deployment issues and keep secrets out of source control. ✅
