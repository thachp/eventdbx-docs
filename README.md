# EventDBX documentation

EventDBX is an event-sourced, NoSQL write-side database that keeps every mutation as an immutable event, guards integrity with Merkle trees, and fans committed changes out through plugins so specialized services can own the read side. This repository powers the public documentation site.

## What’s inside

- **Overview & features** – learn why EventDBX focuses on the write side of CQRS, how schemas, restriction modes, and column definitions work, and what performance looks like up to 10 M records.
- **Quickstart** – install the `dbx` CLI, start the daemon, define schemas, issue tokens, append events, and replicate domains (push/pull/watch).
- **Deployment & integration** – run the published Docker image, attach the TypeScript client, configure encryption keys, and monitor the Prometheus `/metrics` endpoint.
- **Plugin framework** – configure TCP/HTTP/log/process emitters, inspect the RocksDB-backed job queue, replay events, and automate replication.
- **CLI reference** – server lifecycle, configuration, tokens, schemas, aggregates, events, plugins, upgrades, backups, and restores—all grouped in one page.

## Running the docs locally

```bash
npm install -g mint
mint dev
```

Open `http://localhost:3000` to preview changes. Edit navigation, colors, and metadata via `docs.json`.

## Contributing

1. **Report issues** – open a ticket with detailed reproduction steps or ideas.
2. **Fork & clone** – create branches off `develop`.
3. **Develop** – follow the coding standards in this repo; add/update tests where necessary.
4. **Commit** – use [Conventional Commits](https://www.conventionalcommits.org/) (`feat: ...`, `fix: ...`, etc.).
5. **Pull request** – target the upstream `develop` branch, describe the change, and link related issues.

Formatting is handled by the repo-wide Prettier configuration (`.prettierrc.json`) and commit linting via `.commitlintrc.json`.

## License

© 2025 Patrick Thach and contributors. Released under the [MIT License](./LICENSE).
