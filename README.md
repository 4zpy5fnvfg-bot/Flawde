# Flawde

Wrong answers only. But at least they're answers.

## Files
- `public/index.html` — the frontend
- `api/chat.js` — the serverless backend (keeps your API key secret)
- `vercel.json` — Vercel configuration

## Deployment Instructions

### Step 1 — Upload to GitHub
1. Go to github.com and sign in
2. Click the + button (top right) → "New repository"
3. Name it: flawde
4. Leave it Public
5. Click "Create repository"
6. On the next screen, click "uploading an existing file"
7. Upload all three files maintaining the folder structure:
   - vercel.json (root level)
   - api/chat.js
   - public/index.html
8. Click "Commit changes"

### Step 2 — Deploy on Vercel
1. Go to vercel.com and sign in
2. Click "Add New Project"
3. Click "Import" next to your flawde GitHub repository
4. Click "Environment Variables" and add:
   - Name: ANTHROPIC_API_KEY
   - Value: your sk-ant-... key
5. Click "Deploy"
6. Wait ~30 seconds — Vercel gives you a URL like flawde.vercel.app

### Step 3 — Connect flawde.com
1. In Vercel, go to your project → Settings → Domains
2. Add: flawde.com
3. Vercel will show you DNS records to add
4. Log into your domain registrar (Namecheap etc.)
5. Add those DNS records
6. Wait up to 24 hours (usually under 1 hour)

That's it. flawde.com will be live.
