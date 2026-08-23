# coilyco-flight-deck

Open-source tooling for running AI agents you can actually hand authority to.
Built by [Kai Siren](https://coilysiren.me).

The through-line across these projects is the same problem: an agent is only as
safe as the surface you give it. So the surface is declared in a config file,
the boundary is enforced at the call, and every crossing lands in an audit log.

## Install

Four CLIs ship through the flight-deck tap and bucket. Both live on Forgejo
rather than github.com, so brew needs the tap URL spelled out once.

macOS and Linux:

```sh
brew tap coilyco-flight-deck/tap https://forgejo.coilysiren.me/coilyco-flight-deck/homebrew-tap
brew install coilyco-flight-deck/tap/ward
```

Windows:

```powershell
scoop bucket add coilyco-flight-deck https://forgejo.coilysiren.me/coilyco-flight-deck/scoop-bucket
scoop install coilyco-flight-deck/ward
```

Swap `ward` for `specgen`, `agent-compose`, or `aos` to install the others.

## Start here

- **[umbra](https://github.com/coilyco-flight-deck/umbra)** - the occlusion
  framework the rest sits on. You declare the commands an automation may run,
  and umbra validates argv before `execve`, rejects shell metacharacters,
  enforces read/write/delete scope tokens per verb, and appends every call to a
  rotating JSONL audit log. Its `specgen` driver turns a KDL policy plus a
  committed lock into a standalone guarded CLI with no hand-written Go. Start with
  [`examples/`](https://github.com/coilyco-flight-deck/umbra/tree/main/examples),
  one runnable demo per primitive.
- **[ward](https://github.com/coilyco-flight-deck/ward)** - a governed
  execution layer for coding agents. It runs agent work in fresh least-access
  containers and exposes fixed issue, Git, pull-request, broker, log, and
  recovery primitives, so an unattended run leaves a durable issue-to-landing
  trail instead of a mystery. Reach for it when work is separable, concurrent,
  or failure-prone. A single goal agent is simpler for one coherent refactor.
  Pre-1.0 and in active use.
- **[mcp-beaver](https://github.com/coilyco-flight-deck/mcp-beaver)** - renders
  an umbra Guardfile into a guarded MCP server and HTTP tool API, baked into
  one generic OCI image. No per-server Go, no per-server Dockerfile, no
  per-tool input schema. An operation you did not declare has no tool and no
  endpoint, so you can audit one small file and know the blast radius before
  handing a write-capable MCP to an agent.
- **[agent-compose](https://github.com/coilyco-flight-deck/agent-compose)** -
  composes the context an agent harness loads: which role it holds, which
  doctrine and skills come with that role, and which model tier it runs on. One
  canonical source, symlinked into each harness's load point. Ships a
  seven-seat default roster, and an external package can replace it wholesale.
  Claude Code, Codex, Goose, and OpenCode share the same grammar.
- **[agentic-os](https://github.com/coilyco-flight-deck/agentic-os)** - the
  cross-platform host layer underneath all of it. Shared shell and terminal
  configuration for macOS, Linux, and Git-for-Windows, the `aos` launcher, and
  the `aos-precommit` hook suite that validates repository layout, skills,
  documentation shape, and cross-links across the fleet.

## MCP servers

Small, read-only, deliberately bounded adapters. Each one states its exact tool
inventory and what it refuses to do.

- [bluesky-mcp](https://github.com/coilyco-flight-deck/bluesky-mcp) -
  authenticated read-only Bluesky over the AT Protocol SDK. The configured app
  password could authorize writes, so the adapter ships no post, follow, like,
  moderation, or account-mutation tool at all.
- [node-stats-mcp](https://github.com/coilyco-flight-deck/node-stats-mcp) -
  node-local Linux and Kubernetes diagnostics. The node-exporter deployment
  shape, exposing a tool surface instead of Prometheus metrics.
- [reddit-mcp](https://github.com/coilyco-flight-deck/reddit-mcp) - read-only
  private Reddit feeds and public subreddit RSS.
- [lunch-money-k8s](https://github.com/coilyco-flight-deck/lunch-money-k8s) -
  MCP server and Helm chart for the Lunch Money personal-finance API.

## Supporting repositories

- [agent-proxy](https://github.com/coilyco-flight-deck/agent-proxy) -
  observability and trajectory data plane for agent work, OpenAI-compatible in
  front and LiteLLM underneath. In active transition, so treat its interfaces
  as unstable.
- [infrastructure](https://github.com/coilyco-flight-deck/infrastructure) -
  Ansible convergence and k3s manifests for the homelab these tools run on.
- [homebrew-tap](https://github.com/coilyco-flight-deck/homebrew-tap) and
  [scoop-bucket](https://github.com/coilyco-flight-deck/scoop-bucket) - the
  macOS, Linux, and Windows distribution channels, bumped automatically by each
  upstream release.
- [.github](https://github.com/coilyco-flight-deck/.github) - this profile and
  shared review metadata.

Earlier experiments are archived rather than deleted. Browse the
[full repository list](https://github.com/orgs/coilyco-flight-deck/repositories)
to read them.

## Where development happens

[Forgejo](https://forgejo.coilysiren.me/coilyco-flight-deck) is canonical for
development, issues, and releases. GitHub is a verified mirror, and it is the
right place to file a public bug or feature request.

## Elsewhere

- Personal site and writing: [coilysiren.me](https://coilysiren.me)
- Operational back-office: [coilyco-bridge](https://github.com/coilyco-bridge)
- Games, mods, and server tooling: [coilyco-gaming](https://github.com/coilyco-gaming)
