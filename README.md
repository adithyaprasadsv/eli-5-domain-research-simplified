# ELI5 Paper Lab

> AI-powered research paper summariser. Paste an ArXiv URL or upload a PDF — get a structured ELI5 summary ready to push back to this repo as markdown.

## 🚀 Live App

Deployed at: `https://<your-username>.github.io/<your-repo-name>/`

## 🗂 Repo Structure

```
├── index.html              ← The entire app (single file)
├── .github/
│   └── workflows/
│       └── deploy.yml      ← GitHub Actions: injects API key + deploys
├── .gitignore
├── README.md
└── <domain>/               ← Your ELI5 summaries, pushed from the app
    └── paper-title.md
```

## ⚙️ Setup

See deployment steps in the project documentation.

## 🔑 API Key

The Anthropic API key is stored as a GitHub Secret (`ANTHROPIC_API_KEY`) and injected at build time by the GitHub Actions workflow. It is never present in the source code.
