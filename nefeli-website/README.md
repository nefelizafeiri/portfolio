# Nefeli Zafeiri — Personal Website

A personal portfolio website built with [Quarto](https://quarto.org), automatically deployed to GitHub Pages.

## 🚀 Publishing to GitHub Pages (Step-by-Step)

### 1. Install Quarto (one time only)
Download and install from [quarto.org/docs/get-started](https://quarto.org/docs/get-started/).

### 2. Preview locally
```bash
quarto preview
```
This opens a live preview in your browser at `http://localhost:4040`.

### 3. Push to GitHub

Create a new **public** repository on GitHub, then run:

```bash
git init
git add .
git commit -m "Initial website commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
git push -u origin main
```

### 4. Enable GitHub Pages
1. Go to your repo → **Settings** → **Pages**
2. Under **Source**, select **GitHub Actions**
3. Save — that's it! Your site will be live at `https://YOUR_USERNAME.github.io/YOUR_REPO/`

Every time you push to `main`, GitHub Actions will automatically rebuild and deploy your site.

## 📁 Project Structure

```
nefeli-website/
├── _quarto.yml          # Site configuration
├── index.qmd            # Main page content
├── styles.css           # Custom styling
├── docs/                # Generated output (created by quarto render)
└── .github/
    └── workflows/
        └── deploy.yml   # Auto-deploy to GitHub Pages
```
