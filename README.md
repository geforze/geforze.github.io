# All About the Benjamin

Source for my blog, built with [Hugo](https://gohugo.io) using the [Black & Light](https://github.com/davidhampgonsalves/hugo-black-and-light-theme) theme, deployed to https://geforze.github.io via GitHub Actions.

## Writing a new post

```
hugo new content posts/my-post-title.md
```

Edit the new file in `content/posts/`, set `draft: false` when it's ready, then commit and push to `main` — the GitHub Actions workflow builds and deploys automatically.

## Local preview

Install Hugo (extended version) from https://gohugo.io/installation/, then from the repo root:

```
hugo server --buildDrafts
```

Visit http://localhost:1313

## Deployment

Handled by `.github/workflows/hugo.yaml` on every push to `main`. In the repo's Settings → Pages, set "Source" to "GitHub Actions" (one-time setup).
