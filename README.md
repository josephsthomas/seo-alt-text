# Image Alt Text & SEO Filename Generator

## Setup

1. **Clone or unzip** this project.

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Configure your environment**:
   - Copy `.env.example` to `.env` and set `ANTHROPIC_API_KEY`.

4. **Run locally**:
   ```bash
   npm run dev
   ```

5. **Deploy** on Vercel:
   ```bash
   vercel
   ```

## How it works

- Front-end (`index.html`) now calls `/api/claude` instead of directly to Anthropic to avoid CORS errors.
- Serverless function (`api/claude.js`) proxies requests to Anthropic with your API key securely on the server.
