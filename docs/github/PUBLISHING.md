# GitHub Publishing Workflow

## Preconditions

- GitHub CLI (`gh`) installed.
- Valid `gh auth login` session.

## Create and Push Repo (CLI)

```bash
git init
git add .
git commit -m "Initialize TheSibs concept scaffold"
gh repo create thesibs --public --source=. --remote=origin --push
```

## Push Updates

```bash
git add .
git commit -m "Update TheSibs docs and scaffold"
git push -u origin main
```

## Suggested Branch Model

- `main`: stable concept + approved architecture docs.
- `feature/*`: in-flight design or implementation changes.
- Pull request required for architecture and economy contract changes.
