# http-echo — Agent Instructions

## Project Overview

The http-echo component is part of the Pantalasa platform. It provides the
"http-echo" capability and is owned by samuel@pantalasa.org. Primary implementation language:
go.

## Architecture

- Source code lives under the repository root and language-standard directories.
- Deployment is managed via Kubernetes and the ArgoCD manifest in `.argocd/`.
- Service metadata is declared in `pantalasa.json`.

## Build Commands

```bash
go build ./...
go test ./...
golangci-lint run
```

## Testing

- Run the test suite with the commands above before opening a pull request.
- Add tests alongside the code they cover.

## Code Style

- Follow the standard conventions for go.
- Keep functions small and focused; prefer clear names over comments.
- Propagate context and handle errors explicitly.

## Common Patterns

- Configuration via environment variables.
- Structured logging.
- Small, reviewable pull requests referencing a ticket.
