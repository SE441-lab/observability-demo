# Observability Examples

This workspace contains small Go services and local configs that demonstrate observability concepts

## Projects

- `base/`: Minimal service without advanced observability setup.
- `logs/`: Service and Docker setup focused on log collection with Promtail.
- `metrics/`: Service and Prometheus setup focused on metrics scraping.
- `traces/`: Service setup focused on tracing.

## Prerequisites

- Go (1.20+ recommended)
- Docker Desktop (for examples that use `docker-compose.yaml`)

## Run an Example

From the folder you want to run (for example `base/`):

```bash
go run .
```

For folders with Docker Compose support (for example `logs/`, `metrics/`, `traces/`):

```bash
docker compose up --build
```

## Notes

- Each folder is intentionally independent so you can compare setups side by side.
- Some folders include local config files (for example Prometheus or Promtail) that are mounted by Docker Compose.
