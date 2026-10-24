# EST Website

[![Deploy static content to Pages](https://github.com/SPYCrysto/est-website/actions/workflows/static.yml/badge.svg)](https://github.com/SPYCrysto/est-website/actions/workflows/static.yml)
![HTML5](https://img.shields.io/badge/HTML5-Static%20Site-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-Styling-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-Interactive%20UI-F7DF1E?logo=javascript&logoColor=black)
![GitHub Pages](https://img.shields.io/badge/Deployment-GitHub%20Pages-222222?logo=githubpages&logoColor=white)

## Overview

This repository contains a single-page educational website about fast fashion's environmental impact and practical sustainability-focused solutions.

## Features

- Informational sections covering major fast-fashion impact factors
- Expand/collapse “Show Solution” interactions for each topic
- Fully static frontend (no backend dependencies)
- Ready for GitHub Pages deployment through the included workflow

## Tech Stack

- HTML5
- CSS3
- Vanilla JavaScript
- GitHub Actions + GitHub Pages (deployment)

## Project Structure

```text
.
├── .github/workflows/static.yml
└── index.html
```

## Prerequisites

- A modern web browser
- (Optional) Git for cloning
- (Optional) Python 3 for a local static server

## Installation

```bash
git clone https://github.com/SPYCrysto/est-website.git
cd est-website
```

## Development

Quick preview:

- Open `index.html` directly in your browser

Local server (recommended):

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## Testing

There is currently no automated test suite configured in this repository.  
For changes, validate manually by opening the page and verifying layout plus the “Show Solution” toggle behavior.

## Deployment

Deployment is handled by `.github/workflows/static.yml`:

- Trigger: push to `main` (or manual run via `workflow_dispatch`)
- Target: GitHub Pages
- Artifact: repository root uploaded as static content

## Environment Variables

No environment variables are required for local development or deployment of this static site.

## Security Notes

- Do not commit secrets or credentials into this repository.
- This project depends on third-party hosted images referenced by URL in `index.html`; review external resources periodically.

## Contributing

1. Create a feature branch from `main`.
2. Keep changes focused and minimal.
3. Manually verify the page in a browser.
4. Open a pull request with a clear description of the change and screenshots when UI is affected.
