# Enterprise Kubernetes — Personal Brand Website

Personal website for Kubernetes consulting, audit service, course waitlist, and YouTube channel.

## Deploy in 3 steps

### Prerequisites (install once)
- [Git](https://git-scm.com/download/win)
- [GitHub CLI](https://cli.github.com) — then run `gh auth login`
- [Railway CLI](https://docs.railway.app/develop/cli) — `npm install -g @railway/cli`
- [Node.js 18+](https://nodejs.org)

### Option A — One script (PowerShell)
```powershell
cd "C:\Users\ankit\Documents\Claude\Projects\Side Project\enterprise-k8s-website"
.\DEPLOY.ps1
```

### Option B — Manual steps
```powershell
# 1. Init git
git init
git branch -M main
git add .
git commit -m "Initial commit"

# 2. Push to GitHub
gh repo create enterprise-k8s-website --public --source=. --remote=origin --push

# 3. Deploy to Railway
railway login
railway init --name enterprise-k8s-website
railway up
```
