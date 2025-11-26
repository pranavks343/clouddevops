# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) (or [oxc](https://oxc.rs) when used in [rolldown-vite](https://vite.dev/guide/rolldown)) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.

## CI/CD Deployment

This project uses GitHub Actions for automated CI/CD. The workflow automatically builds and deploys the frontend to GitHub Pages on every push to the `main` branch.

### Setup Instructions

1. **Enable GitHub Pages**:
   - Go to your repository Settings → Pages
   - Under "Source", select "GitHub Actions"

2. **Workflow Details**:
   - The workflow file is located at `.github/workflows/deploy.yml`
   - It triggers on:
     - Push to `main` branch
     - Manual workflow dispatch
   - Builds the project using `npm run build`
   - Deploys the `dist` folder to GitHub Pages

3. **Access Your Deployed Site**:
   - After the first successful deployment, your site will be available at:
     `https://[username].github.io/travel-frontend/`
   - The deployment URL will be shown in the Actions tab after each successful run

### Manual Deployment

You can also manually trigger the deployment by:
- Going to the Actions tab in your repository
- Selecting the "Build and Deploy Frontend" workflow
- Clicking "Run workflow"
