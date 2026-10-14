+++
title = "Projects"
path = "projects"
template = "page.html"
+++

```sh
Let's build something.
```

<div class="wrap-collabsible">
  <input id="collapsible-cerebrum" class="toggle" type="checkbox">
  <label for="collapsible-cerebrum" class="lbl-toggle">cerebrum <em>(self-hosted second brain)</em></label>
  <div class="collapsible-content">
    <div class="content-inner">
      <p>A self-hosted second brain: notes are plain markdown files on disk, cross-referenced with standard markdown links, with a visual graph of how they connect. No lock-in, the vault is just a folder.</p>
      <ul>
        <li><strong>plain-markdown vault</strong> backed by a SQLite index that can always be rebuilt from disk</li>
        <li><strong>graph view and backlinks</strong> to see how notes connect</li>
        <li><strong>full-text search</strong> with SQLite FTS5 and bm25 ranking</li>
        <li><strong>three clients</strong>: a React web app, an installable PWA with offline reading, and a Tauri desktop app for Linux</li>
        <li><strong>auth</strong> with accounts, JWT sessions, and personal API tokens</li>
        <li><strong>CI pipeline</strong> running ruff, pylint, mypy --strict, pytest, biome, tsc, and vitest on every PR</li>
      </ul>
      <p>Built with Python, FastAPI, SQLite, React, TypeScript, Tauri, and Docker Compose.</p>
      <p><a href="https://github.com/piurizza/cerebrum">github.com/piurizza/cerebrum</a></p>
    </div>
  </div>
</div>

<div class="wrap-collabsible">
  <input id="collapsible-master-companion" class="toggle" type="checkbox">
  <label for="collapsible-master-companion" class="lbl-toggle">master-companion <em>(work in progress)</em></label>
  <div class="collapsible-content">
    <div class="content-inner">
      <p>A local LLM companion for tabletop RPG game masters. Point it at your game's manual and ask about rules, NPCs, or world-building: it runs entirely on your machine and answers from the manual, not from generic fantasy knowledge.</p>
      <ul>
        <li><strong>synthetic roster chunks</strong>: "which classes are there?" has no single passage that answers it, so lists scattered across the manual are collected into dedicated chunks at index time</li>
        <li><strong>page references</strong>: mention "page 112" and that page is pulled into the context next to the semantic matches</li>
        <li><strong>strict grounding</strong>: the model answers only from retrieved excerpts, says so when the manual is silent, and flags concepts borrowed from other games</li>
        <li><strong>PDF cleanup pipeline</strong> for real-world manuals: front matter, indexes, running headers, and watermarks stripped before chunking</li>
        <li><strong>game-agnostic</strong>: every system, language, and cleanup rule lives in a YAML config</li>
      </ul>
      <p>Built with Python 3.12, llama.cpp, sentence-transformers, FAISS, and Streamlit.</p>
      <p><a href="https://github.com/piurizza/master-companion">github.com/piurizza/master-companion</a></p>
    </div>
  </div>
</div>

<div class="wrap-collabsible">
  <input id="collapsible-mffbg" class="toggle" type="checkbox">
  <label for="collapsible-mffbg" class="lbl-toggle">my_fantastic_first_board_game <em>(coming soon)</em></label>
  <div class="collapsible-content">
    <div class="content-inner">
      <p>A card game built from scratch: game engine, simulations, balancing, and a web server for playtesting. Instead of manually tweaking numbers until things "feel right," RL agents play thousands of games and the math tells you what's balanced.</p>
      <ul>
        <li><strong>custom game engine</strong> supporting 2 to 5 players</li>
        <li><strong>self-play RL agents</strong> that learn strategy through millions of simulated games</li>
        <li><strong>multi-phase tuning pipeline</strong>: 2,000+ configurations narrowed down to a single champion</li>
        <li><strong>composite balance scoring</strong> across win fairness, entropy, player influence, and game stretch</li>
        <li><strong>web server</strong> for live playtesting with the tuned configuration</li>
      </ul>
      <p>Built with Python, PostgreSQL, and a lot of patience.</p>
    </div>
  </div>
</div>

<div class="wrap-collabsible">
  <input id="collapsible-gazzetta" class="toggle" type="checkbox">
  <label for="collapsible-gazzetta" class="lbl-toggle">gazzetta-newsletter <em>(concorsi pubblici aggregator)</em></label>
  <div class="collapsible-content">
    <div class="content-inner">
      <p>An automated pipeline that aggregates Italian public contest listings from multiple official sources and delivers a filtered newsletter via email.</p>
      <ul>
        <li><strong>multi-source retrieval</strong> from official government feeds and APIs (e.g. Gazzetta Ufficiale, InPA)</li>
        <li><strong>fuzzy keyword matching</strong> using Levenshtein distance to filter relevant contests across all sources</li>
        <li><strong>domain-driven design</strong> with independent retriever packages, shared pipeline kernel, and dependency injection</li>
        <li><strong>Gmail API integration</strong> for automated email delivery with results grouped by source</li>
        <li><strong>CI pipeline</strong> running ruff, mypy, and pytest on every PR</li>
      </ul>
      <p>Built with Python 3.13, feedparser, requests, and marshmallow-dataclass.</p>
      <p><a href="https://github.com/piurizza/gazzetta-newsletter">github.com/piurizza/gazzetta-newsletter</a></p>
    </div>
  </div>
</div>

<div class="wrap-collabsible">
  <input id="collapsible-gdaf" class="toggle" type="checkbox">
  <label for="collapsible-gdaf" class="lbl-toggle">gdaf <em>(geospatial data analysis framework)</em></label>
  <div class="collapsible-content">
    <div class="content-inner">
      <p>A web framework for searching, downloading, and analyzing satellite imagery. Born as a Master's thesis, then hardened with security fixes, modern tooling, and proper test coverage.</p>
      <ul>
        <li><strong>satellite imagery search</strong> via the Planet API (PlanetScope Ortho Visual), filtered by GeoJSON area of interest and date range</li>
        <li><strong>map lab</strong> for viewing downloaded TIFF rasters as PNG with coordinate metadata reprojected to WGS84</li>
        <li><strong>OpenStreetMap integration</strong> loading vector data into DuckDB for spatial queries</li>
        <li><strong>full auth flow</strong> with email verification, password recovery, CSRF protection, and secure hashing</li>
        <li><strong>CI pipeline</strong> running ruff, mypy, and pytest on every PR</li>
      </ul>
      <p>Built with Python 3.12, Flask, PostgreSQL, GDAL, Docker Compose, and Alembic.</p>
      <p><a href="https://github.com/piurizza/gdaf">github.com/piurizza/gdaf</a></p>
    </div>
  </div>
</div>
