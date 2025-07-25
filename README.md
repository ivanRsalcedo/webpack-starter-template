# Webpack Starter Template

A thing to clone because life's too short!!

Includes: `index.js`, `style.css`, and `template.html`

---

## Quick Setup

`<name>` is the name of your new repo.

Clone template, strip old Git history, boot up project.

```bash
cp -r webpack-starter-template <name>
cd <name>
rm -rf .git
git init
npm install
code .
```

---

## Dev Commands

```bash
npm start
```
```
npm run build 
```
---

## GitHub Pages Deploy

### First time only:

Make branch to deploy from.

```bash
git branch gh-pages
```

### Every time you deploy:

Run this ritual after making changes you want to publish live.

```bash
git checkout gh-pages && git merge main --no-edit
npm run build
git add dist -f && git commit -m "Deployment commit"
git subtree push --prefix dist origin gh-pages
git checkout main
```

> Also, check if GitHub Pages is set to deploy from `gh-pages` in **Settings → Pages → Source/Branch**.
