# Zephyrix Social Media Strategy — Deployment Guide

## Project Structure
```
zephyrix-strategy/
├── package.json
├── public/
│   └── index.html
├── src/
│   ├── index.js
│   └── App.jsx       ← All strategy content lives here
└── README.md
```

---

## Option 1: Deploy to Vercel (Recommended — Free, 3 mins)

### Step 1 — Install Node.js
Download from: https://nodejs.org (choose LTS version)

### Step 2 — Upload to GitHub
1. Go to https://github.com and create a free account (if you don't have one)
2. Click **New repository** → name it `zephyrix-strategy` → click **Create repository**
3. Upload all files from this folder by dragging them into the GitHub interface
   OR use Git commands:
   ```bash
   git init
   git add .
   git commit -m "Zephyrix strategy"
   git remote add origin https://github.com/YOUR_USERNAME/zephyrix-strategy.git
   git push -u origin main
   ```

### Step 3 — Deploy on Vercel
1. Go to https://vercel.com and sign up with your GitHub account
2. Click **Add New Project**
3. Select your `zephyrix-strategy` repository
4. Click **Deploy** (Vercel auto-detects React — no configuration needed)
5. Done! Your URL will be: `https://zephyrix-strategy.vercel.app`

---

## Option 2: Deploy to Netlify (Alternative — Also Free)

### Step 1 — Build the project locally
```bash
# Install dependencies
npm install

# Build the production files
npm run build
```
This creates a `build/` folder.

### Step 2 — Deploy to Netlify Drop
1. Go to https://netlify.com/drop
2. Drag and drop the entire `build/` folder onto the page
3. Done! You get a URL like `https://random-name.netlify.app`
4. Optional: Click **Claim your site** to customize the URL

---

## Option 3: CodeSandbox (Fastest — No install needed)

1. Go to https://codesandbox.io
2. Click **New Sandbox** → Select **React**
3. Delete the default `App.js` file
4. Create `App.jsx` and paste the contents of `src/App.jsx`
5. Update `index.js` to match the file in `src/index.js`
6. Click **Share** (top right) → **Copy link**
7. Done! Share the link with your team

---

## Option 4: Run Locally (Preview before deploying)

```bash
# Install dependencies (only needed once)
npm install

# Start the local development server
npm start
```

Opens automatically at: http://localhost:3000

---

## Customising the Content

All strategy content is in **`src/App.jsx`**.

| What to change | Where to find it |
|---|---|
| Trend descriptions & stats | `trends` array at the top |
| Post examples & hooks | Inside each trend's `platforms` object |
| Calendar content | `calendarData` array |
| Trend tools | `trendTools` array |
| Platform do's & don'ts | Inside the Platform Guide section |
| Brand name / colours | Search for "Zephyrix" and the colour codes |

---

## Common Issues

**"npm: command not found"**
→ Install Node.js from https://nodejs.org first

**"Module not found"**
→ Run `npm install` in the project folder first

**Vercel build fails**
→ Make sure all files are uploaded including `package.json` and the `public/` folder

---

Built for: Zephyrix Performance Marketing Agency
Strategy Period: March–April 2026
