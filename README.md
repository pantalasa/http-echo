http-echo
=========
HTTP Echo is a small go web server that serves the contents it was started with
as an HTML page.

The default port is 5678, but this is configurable via the `-listen` flag:

```
http-echo -listen=:8080 -text="hello world"
```

Then visit http://localhost:8080/ in your browser.

## Project Overview

The http-echo component provides the "http-echo" capability for the Pantalasa
platform. It is owned by samuel@pantalasa.org and implemented primarily in go.

## Installation

Clone the repository and install dependencies using the standard go
toolchain.

## Usage

Build and run using the commands documented in [AGENTS.md](AGENTS.md).

## Project Structure

| Path | Purpose |
|------|---------|
| `pantalasa.json` | Service manifest (owner, domain, deployment) |
| `.argocd/` | ArgoCD Application manifest |
| `AGENTS.md` | Agent / contributor instructions |

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). Security policy: [SECURITY.md](SECURITY.md).

## License

Released under the MIT License — see [LICENSE](LICENSE).
