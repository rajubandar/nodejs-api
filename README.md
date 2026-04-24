# nodejs-api

A simple Node.js REST API packaged with Docker.

## Endpoints

- `GET /health` — returns `{ "status": "OK" }`

## Docker Setup

### Build the image

```bash
docker build -t nodejs-api .
```

### Run the container

```bash
docker run -p 8080:8080 nodejs-api
```

Verify: `curl http://localhost:8080/health`

### Run with docker compose

```bash
docker compose up -d
```
