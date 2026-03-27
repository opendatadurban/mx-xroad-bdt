# MX X-Road Bulk Data Transfer — Releases

This repository hosts the release artifacts for the **MzansiXchange (MX) Bulk Data Transfer (BDT)** system — a resumable file transfer solution built on the [TUS protocol](https://tus.io) and designed to operate over the [X-Road](https://x-road.global/) secure data exchange layer.

## What's Here

GitHub Releases in this repo contain all deployment artifacts:

| Artifact | Description |
|----------|-------------|
| **Docker image** | `ghcr.io/opendatadurban/bdt-api:{version}` (public GHCR package, not attached here) |
| **Docker deployment kit** | `bdt-docker-kit-{version}.zip` — docker-compose.yml, .env.example, deployment README |
| **Native API (Linux)** | `bdt-api-{version}-linux-x64.tar.gz` — API + bundled Node.js + PM2 |
| **Native API (Windows)** | `bdt-api-{version}-windows-x64.zip` — API + bundled Node.js + PM2 |
| **CLI (Linux)** | `bdt-linux-amd64` — standalone binary |
| **CLI (Windows)** | `bdt-windows-amd64.exe` — standalone binary |

## Getting Started

1. Go to the [latest release](https://github.com/opendatadurban/mx-xroad-bdt/releases/latest)
2. Download the **Docker deployment kit** or **Native API package** for your platform
3. Download the **CLI binary** for your platform
4. Follow the README included in the deployment kit

## Deployment Options

- **Docker (recommended):** Use the Docker deployment kit with `docker compose up -d`
- **Native:** Extract the native package — includes bundled Node.js and PM2, no system dependencies required

## Documentation

Detailed deployment guides, CLI usage, and X-Road configuration instructions are included in each release's deployment kit.
## About

BDT enables government departments connected to the MzansiXchange X-Road network to transfer large datasets (20GB–2TB+) reliably using resumable uploads. Transfers can be paused, resumed, and monitored via the CLI or API.

Built and maintained by [Open Cities Lab](https://opendata.durban).
