<div align="center">
  <br>
  <h1>Reverse Artist Search</h1>
  <p>
    <strong>A dedicated, multi-engine reverse image search tool for tracking down original artists and high-resolution sources.</strong>
  </p>
  <p>
    <a href="https://reverse-art-search.pages.dev/"><img src="https://img.shields.io/website?url=https%3A%2F%2Freverse-art-search.pages.dev&up_message=online&up_color=success&style=for-the-badge&logo=cloudflare&label=Live%20Demo" alt="Live Demo"></a>
    <a href="https://github.com/DevilNine"><img src="https://img.shields.io/badge/Made_by-DevilNine-dc2626?style=for-the-badge" alt="Made by DevilNine"></a>
    <a href="https://ko-fi.com/devilnine"><img src="https://img.shields.io/badge/Support_on-Ko--fi-f97316?style=for-the-badge&logo=kofi&logoColor=white" alt="Support on Ko-fi"></a>
  </p>
</div>

<br>

## Overview

Finding the original creator of a piece of art can be difficult, especially when the image has been reposted, compressed, or cropped multiple times. **Reverse Artist Search** solves this by concurrently querying multiple specialized search engines (like SauceNAO, IQDB, Google Lens, and Yandex) and aggregating the results in a single, unified interface.

This repository hosts the obfuscated, production-ready frontend build. The application is deployed as a Serverless Single Page Application (SPA).

🔗 **Live Demo:** [reverse-art-search.pages.dev](https://reverse-art-search.pages.dev/)

## Core Capabilities

* **Concurrent Source Queries**: Dispatches search requests across multiple engines simultaneously to maximize match probability.
* **Unified Results Dashboard**: Aggregates and normalizes responses from different sources into a single, structured list.
* **Intelligent History Persistence**: Maintains a local history of recent searches and uploads, allowing users to return to previous results seamlessly without re-uploading.
* **Production-Grade UI**: Responsive interface designed with attention to accessible touch targets and visual hierarchy.

## System Architecture

* **Frontend**: React + Vite. Deployed as a static SPA on Cloudflare Pages.
* **State Management**: React hooks for local state and session tracking.
* **Backend Communication**: Designed to communicate with an external REST API (FastAPI + Python). 

> **Note regarding the Backend**: Because the backend handles heavy operations (PyTorch for image hashing, headless browser automation via Playwright), it is hosted on a separate compute server. This frontend repository communicates with that server via environment variables.

---

<div align="center">
  <p><i>Made for artists, by <a href="https://github.com/DevilNine">DevilNine</a></i></p>
  <a href="https://ko-fi.com/devilnine">
    <img src="https://ko-fi.com/img/githubbutton_sm.svg" alt="Support me on Ko-fi">
  </a>
</div>
