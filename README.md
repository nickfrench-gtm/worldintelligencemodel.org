# World Intelligence Model

Public placeholder for the World Intelligence Model research institution.

This repository is intentionally independent from the WIM reference implementation. It contains no product code, backend, API, authentication, or runtime integration.

## Production

- Fly application: `world-intelligence-model`
- URL: https://world-intelligence-model.fly.dev

## Stack

- Semantic HTML
- CSS
- Nginx 1.27 Alpine
- Docker
- Fly.io

## Local preview

```sh
docker build -t world-intelligence-model-site .
docker run --rm -p 8080:80 world-intelligence-model-site
```

Open `http://localhost:8080`.

## Deploy

```sh
flyctl deploy
```

The Fly application name is declared in `fly.toml`. Custom-domain DNS is intentionally not configured in this session.

## Structure

```text
.
├── Dockerfile
├── fly.toml
├── nginx.conf
└── site
    ├── index.html
    ├── styles.css
    ├── mission/index.html
    ├── research-roadmap/index.html
    ├── publications/index.html
    ├── publications/working-paper-001/index.html
    ├── benchmarks/index.html
    ├── experiment-registry/index.html
    ├── governance/index.html
    └── license/index.html
```
