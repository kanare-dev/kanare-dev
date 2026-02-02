# Release: resume PDF

This repository generates `resume.pdf` from `resume.adoc` via GitHub Actions, and publishes it as a GitHub Release asset.

## Download URL (latest)

`https://github.com/Canale0107/Canale0107/releases/latest/download/resume.pdf`

## How to publish a new PDF

1) Update `resume.adoc` (and/or `pdf/theme.yml`) on `main`.

2) Create a version tag and push it.

```bash
git tag v1.0.0
git push origin v1.0.0
```

3) GitHub Actions will:

- build `dist/resume.pdf`
- create/update the Release for the tag
- upload `resume.pdf` to the Release assets

## Workflow

- `.github/workflows/resume-pdf.yml`
