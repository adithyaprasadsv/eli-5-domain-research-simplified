# ELI5 Paper Lab

> AI-powered research paper summariser. Paste an ArXiv URL or upload a PDF — get a structured ELI5 summary and push it directly to this repo as a markdown file.

## Live App

`https://adithyaprasadsv.github.io/eli-5-domain-research-simplified/`

## First-Time Setup

1. Open the live app
2. Click **Settings** in the sidebar
3. Enter your **Anthropic API key** (from console.anthropic.com)
4. Optionally enter your **GitHub token** and repo details to enable direct push
5. Click **Save Settings**

Keys are stored in `sessionStorage` only — they clear when you close the tab and are never sent anywhere except the respective APIs.

## Repo Structure

```
├── index.html                 ← Entire app (single file)
├── .github/workflows/
│   └── deploy.yml             ← GitHub Pages deployment
├── .gitignore
├── README.md
└── supply-chain/              ← ELI5 summaries pushed from the app
    └── paper-title.md
```

## No API Keys in Code

The Anthropic API key is entered by the user at runtime in the Settings page. Nothing sensitive is ever committed to this repo.
