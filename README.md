# Homepage Dashboard

Self-hosted [Homepage](https://gethomepage.dev/) dashboard deployed via Docker Compose.

## Quick Start

```bash
docker compose up -d       # Start (or restart after config changes)
docker compose down        # Stop
docker compose logs -f     # Tail logs
```

Dashboard is accessible at `http://localhost:3000`.

## Configuration

Configuration changes to YAML files are hot-reloaded without container restart.

- **services.yaml** — Dashboard tiles (service groups and links)
- **bookmarks.yaml** — Bookmark categories
- **widgets.yaml** — Top-bar widgets (search, system stats, weather)
- **settings.yaml** — Global settings and API keys (excluded from version control)
- **docker.yaml** — Docker socket integration for container auto-discovery
- **proxmox.yaml** — Proxmox VE integration
- **kubernetes.yaml** — Kubernetes integration
- **custom.css** — CSS overrides
- **custom.js** — JS overrides

## Documentation

See [gethomepage.dev/configs/](https://gethomepage.dev/configs/) for configuration documentation.
