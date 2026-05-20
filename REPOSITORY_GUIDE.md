# Repository Guide

This repository is generated from the Unicorn Rank local build output.

## Update Workflow

```bash
node scripts/build-site.mjs
node scripts/export-github-dataset.mjs
cd exports/unicorn-rank-datasets
git status
git add .
git commit -m "Update dataset snapshot 2026-05-18"
git push
```

## Repository Shape

- `README.md`: public entrypoint for humans and AI crawlers.
- `index.json`: machine-readable dataset index.
- `manifest.json`: byte sizes and sha256 hashes for exported files.
- `latest/`: moving pointer to newest data.
- `snapshots/2026-05-18/`: date-stamped immutable snapshot.
- `rankings/`: Markdown pages for GitHub search and human browsing.
- `reports/`: weekly report Markdown.

## Why This Helps AI

GitHub adds an external, crawlable, versioned mirror. AI systems can discover the project through web search, inspect stable JSON files, compare history through commits, and verify the dataset using hashes.
