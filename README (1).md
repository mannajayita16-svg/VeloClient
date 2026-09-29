# VeloClient

A polished client-operations website inspired by the supplied reference design.

## Included

- Responsive landing page
- Dark premium SaaS visual style
- Dashboard mockup
- Feature and pricing sections
- Login modal
- Demo client portal
- Gemini AI assistant endpoint
- Support and PayPal contact details
- Vercel-ready serverless API

## Important: Gemini API key

Do **not** paste your Gemini API key into `app.js` or `index.html`.

For Vercel:

1. Push this folder to a GitHub repository.
2. Import the repository into Vercel.
3. In Vercel, open **Project Settings → Environment Variables**.
4. Add:
   - Name: `GEMINI_API_KEY`
   - Value: your Gemini API key
5. Redeploy.

The browser calls `/api/gemini`, and the secret stays on the server.

## Login

The included login is a front-end demo. It stores the entered email in localStorage and opens the portal. It is NOT production authentication.

For real customer accounts, connect the UI to a real authentication/database provider before accepting sensitive customer information.

## Payment

The site displays:

- PayPal contact: `jayita5628@gmail.com`
- Support: `anikmanna697@gmail.com`

An email address alone is not a verified PayPal checkout integration. For real payments, use a PayPal checkout/merchant integration and keep its credentials server-side.

## GitHub deployment

The landing page can be hosted as static files, but the Gemini endpoint requires a serverless host such as Vercel. For the easiest full deployment, use Vercel connected to GitHub.
