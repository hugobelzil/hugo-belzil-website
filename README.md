# Hugo Belzil Academic Website

Static academic website built with Jekyll for GitHub Pages. The structure is
inspired by academic themes such as al-folio, but kept small so it is easy to
edit and deploy.

## Edit Content

- Home page: `index.html`
- Research: `research.md`
- CV: `cv.md`
- Notes: `_posts/`
- Navigation: `_data/navigation.yml`
- Site settings: `_config.yml`

## LaTeX

Set `math: true` in a page or post front matter to load MathJax.

Inline math:

```tex
$\alpha + \beta$
```

Display math:

```tex
$$
\hat{\theta} = \arg\min_\theta Q_n(\theta)
$$
```

## Run Locally

Install Ruby, then run:

```sh
bundle install
bundle exec jekyll serve
```

Open `http://127.0.0.1:4000`.

## Deploy

The included GitHub Actions workflow builds and deploys the site from `main`.
In the repository settings, set GitHub Pages to deploy from GitHub Actions.
