# `netlify-cli` V10 breaks React Fast Refresh - minimal reproduciton

Steps to reproduce:

1. Run `npm start`
2. Change something, like JSX, in `src/pages/index.js`
3. Observe that it does not hot-reload in the browser
4. Browse to `http://localhost:8000` (the underlying Gatsby dev server)
5. Try again; observe that Fast Refresh is working fine
6. Downgrade to `netlify-cli@^9`
7. Browse to `http://localhost:8888` (the `netlify-cli` dev server)
8. Try again; observe that Fast Refresh is working fine
