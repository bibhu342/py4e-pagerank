# Py4E PageRank Capstone
Builds a basic web spider, stores crawled pages in SQLite, computes PageRank, and visualizes top 25 nodes using D3.js force graph.

## Steps Completed
- Crawled `python-data.dr-chuck.net` (~150 pages)
- Crawled `docs.python.org` (~100 pages)
- Ran PageRank (`sprank.py`)
- Dumped top-ranked URLs (`spdump.py`)
- Visualized graph (`force.html`, D3.js)

## Screenshots
- drchuck_spdump_terminal.png
- drchuck_force_25.png
- othersite_spdump_terminal.png
- othersite_force_25.png

## Tools
- Python 3
- SQLite
- BeautifulSoup
- D3.js
- VS Code

## Live Demo
View the 25-node force graph from Run 2 on GitHub Pages: <your-pages-url>

## Reproduce Locally
```bash
python -m venv .venv
. .venv/Scripts/Activate.ps1  # Windows
pip install beautifulsoup4
python spider.py   # crawl
python sprank.py   # pagerank
python spdump.py   # dump
python spjson.py   # build spider.js (enter 25)
# open force.html in a browser

## 4) Tag a release
Looks professional and lets you reference this assignment cleanly.

```bash
git tag v1.0.0 -m "Py4E PageRank capstone"
git push origin v1.0.0

MIT License

Copyright (c) 2025 Bibhudendu Behera

Permission is hereby granted, free of charge, to any person obtaining a copy...
