# Pushing this site to GitHub

I prepped a clean first commit but couldn't push it from here — there's no GitHub MCP connector available in your environment, and I can't authenticate to your GitHub account without one. Two ways to get this to GitHub from your machine:

## Option A — Fastest (GitHub CLI)

If you have `gh` installed and authenticated (`gh auth login`), from this folder run:

```sh
gh repo create gate8-brochure --private --source=. --push
```

That creates a private `gate8-brochure` repo on your account and pushes everything in one shot.

If you don't have `gh`:

```sh
brew install gh
gh auth login
```

## Option B — Manual

1. Go to https://github.com/new and create an empty private repo called `gate8-brochure` (don't add a README — we already have one).
2. From this folder:

```sh
git init -b main
git add .
git commit -m "Initial commit: GATE8 brochure site"
git remote add origin git@github.com:<your-username>/gate8-brochure.git
git push -u origin main
```

(Swap `git@github.com:...` for the HTTPS URL if you don't use SSH keys.)

## Option C — Use the bundle I made

Alongside this folder I dropped `gate8-brochure.bundle` — a single-file git bundle with the first commit already in it. You can `git clone gate8-brochure.bundle` to get a working copy with history, then set up a remote and push as above. Useful if you want the exact commit I prepared, not a fresh one.
