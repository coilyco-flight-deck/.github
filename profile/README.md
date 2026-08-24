# coilyco-flight-deck

Open-source agent tooling by [Kai Siren](https://coilysiren.me). The recurring
problem across these projects is that an agent is only as safe as the surface
you hand it, so the surface gets declared in a config file and enforced at the
call.

## Projects

- **[agent-compose](https://github.com/coilyco-flight-deck/agent-compose)** -
  selects roles, personalities, skills, and tool inventories, then emits an
  inspectable bundle. No executable authority rides along. Installs as
  `acompose`, and Claude Code, Codex, Goose, and OpenCode share the grammar.
- **[umbra](https://github.com/coilyco-flight-deck/umbra)** - a config driven
  occlusion framework that puts explicit boundaries around CLIs and APIs. It
  validates argv before `execve`, checks a scope token per verb, and appends
  every call to a rotating audit log. Its `specgen` driver turns a KDL policy
  into a standalone guarded CLI with no hand-written Go.
- **[mcp-beaver](https://github.com/coilyco-flight-deck/mcp-beaver)** - renders
  a guardfile into a guarded MCP server and HTTP tool API. One generic runtime,
  many guardfiles, and an undeclared operation has no handler at all. Ships as
  an image plus a Helm chart, so deploying one is a values file.

A fourth, [sirens-echo](https://github.com/coilyco-gaming/sirens-echo), lives
over in [coilyco-gaming](https://github.com/coilyco-gaming).

## Install

`agent-compose`, `specgen`, `ward`, and `aos` install from a Forgejo-hosted tap
or bucket, so the URL is spelled out once.

```sh
brew tap coilyco-flight-deck/tap https://forgejo.coilysiren.me/coilyco-flight-deck/homebrew-tap
brew install coilyco-flight-deck/tap/agent-compose
```

```powershell
scoop bucket add coilyco-flight-deck https://forgejo.coilysiren.me/coilyco-flight-deck/scoop-bucket
scoop install coilyco-flight-deck/agent-compose
```

mcp-beaver is not a CLI. It ships as an image and Helm chart.

## MCP servers

Small read-only adapters. Each states its exact tool inventory and what it
refuses to do.

- [bluesky-mcp](https://github.com/coilyco-flight-deck/bluesky-mcp) -
  authenticated Bluesky, with no write tool at all.
- [node-stats-mcp](https://github.com/coilyco-flight-deck/node-stats-mcp) -
  node-local Linux and Kubernetes diagnostics.
- [reddit-mcp](https://github.com/coilyco-flight-deck/reddit-mcp) - private
  Reddit feeds and public subreddit RSS.
- [lunch-money-k8s](https://github.com/coilyco-flight-deck/lunch-money-k8s) -
  the Lunch Money API, with a Helm chart.

## Also here

- [ward](https://github.com/coilyco-flight-deck/ward) - governed execution
  layer for coding agents. Runs agent work in isolated containers and records
  an audit trail.
- [agentic-os](https://github.com/coilyco-flight-deck/agentic-os) - the host
  layer the rest of this runs on: shell and terminal configuration, the `aos`
  launcher, and the `aos-precommit` hook suite. A reference implementation
  rather than something to adopt.
- [agent-proxy](https://github.com/coilyco-flight-deck/agent-proxy) -
  observability and trajectory data plane for agent work. In active transition,
  so its interfaces are unstable.
- [infrastructure](https://github.com/coilyco-flight-deck/infrastructure) -
  Ansible convergence and k3s manifests for the homelab.
- [homebrew-tap](https://github.com/coilyco-flight-deck/homebrew-tap) and
  [scoop-bucket](https://github.com/coilyco-flight-deck/scoop-bucket) - the
  distribution channels, bumped by each upstream release.

Earlier experiments are archived rather than deleted. The
[full repository list](https://github.com/orgs/coilyco-flight-deck/repositories)
has them.

## Elsewhere

[Forgejo](https://forgejo.coilysiren.me/coilyco-flight-deck) is canonical for
development, issues, and releases. GitHub is a verified mirror and the right
place to file a public bug.

- [coilysiren.me](https://coilysiren.me) - personal site and writing
- [coilyco-gaming](https://github.com/coilyco-gaming) - games, mods, and server tooling
- [coilyco-bridge](https://github.com/coilyco-bridge) - operational back-office
