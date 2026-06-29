# Awesome World Model Hub

A curated hub for world model papers, benchmarks, datasets, and research.

This repository is generated and maintained with
[awesome-hub-generator](https://github.com/jin-s13/awesome-hub-generator).

## Daily update

The GitHub Actions workflow in `.github/workflows/daily-update.yml` runs every
day at UTC 00:00 / Beijing 08:00. It refreshes papers, datasets, teaser images,
OpenAlex citation metadata, deep research notes, and the Astro website.

Required repository secret:

- `ARK_API_KEY`

Optional repository secrets:

- `ARK_API_BASE_URL`
- `ARK_MODEL_NAME`
- `SMART_MODEL_NAME`
- `MINERU_API_KEY`
- `OPENALEX_API_KEY`
- `OPENALEX_MAILTO`

Optional repository variable:

- `GENERATOR_REPO=jin-s13/awesome-hub-generator`

## Local preview

```bash
python awesome-hub-generator/scripts/build.py --data-dir data --output website --render-only --skip-build
cd website
npm install
npm run dev
```
