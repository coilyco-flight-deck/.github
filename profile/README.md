# coilyco-flight-deck

Public OSS portfolio of Kai Siren.

Focus: LLM observability, agent devex, tooling for AI consumers.

## Headline projects

- **[o2r (otel-a2a-relay)](https://github.com/coilyco-flight-deck/otel-a2a-relay)** - OpenTelemetry relay for the A2A agent protocol. Translates JSON-RPC 2.0 agent calls into OTel spans exported to Phoenix, Tempo, and Grafana.
- **[gauntlet](https://github.com/coilyco-flight-deck/gauntlet)** - Adversarial MCP server and Claude Code plugin that stress-tests HTTP APIs under sustained two-role (Attacker plus Inspector) attack.
- **[repo-recall](https://github.com/coilyco-flight-deck/repo-recall)** - Rust hydration layer joining git, gh, and Claude Code session history into a local-first MCP and HTTP surface. Published via Homebrew tap.
- **[cli-guard](https://github.com/coilyco-flight-deck/cli-guard)** - Go security-boundary framework for urfave/cli - audit logging, scope tokens, and allowlist enforcement.

## Repositories

- [`coilyco-flight-deck/.github`](https://github.com/coilyco-flight-deck/.github) - Organization profile for public AI-agent tooling, observability, and developer-platform projects.
- [`coilyco-flight-deck/agent-compose`](https://github.com/coilyco-flight-deck/agent-compose) - Context compiler that composes roles, personalities, skills, and tool inventories for AI-agent harnesses.
- [`coilyco-flight-deck/agent-proxy`](https://github.com/coilyco-flight-deck/agent-proxy) - Observability and trajectory data plane for AI agents with OpenAI-compatible proxying and LiteLLM.
- [`coilyco-flight-deck/agentic-os`](https://github.com/coilyco-flight-deck/agentic-os) - Cross-platform agentic operating layer with dotfiles, skills, guarded tooling, and repository validators.
- [`coilyco-flight-deck/bluesky-mcp`](https://github.com/coilyco-flight-deck/bluesky-mcp) - Authenticated read-only Bluesky MCP with a fixed, bounded AT Protocol tool surface.
- [`coilyco-flight-deck/cli-guard`](https://github.com/coilyco-flight-deck/cli-guard) - Security framework for guarded command-line tools with scoped authority, validation, and audit logs.
- [`coilyco-flight-deck/homebrew-tap`](https://github.com/coilyco-flight-deck/homebrew-tap) - Homebrew tap for coilyco-flight-deck tools with automated formula updates.
- [`coilyco-flight-deck/infrastructure`](https://github.com/coilyco-flight-deck/infrastructure) - Infrastructure-as-code for Kai's hosts and Kubernetes homelab, including Ansible convergence and observability.
- [`coilyco-flight-deck/lunch-money-k8s`](https://github.com/coilyco-flight-deck/lunch-money-k8s) - MCP server and Helm chart for the Lunch Money personal-finance API.
- [`coilyco-flight-deck/node-stats-mcp`](https://github.com/coilyco-flight-deck/node-stats-mcp) - Read-only MCP for Linux and Kubernetes diagnostics with bounded host introspection and OTLP export.
- [`coilyco-flight-deck/reddit-mcp`](https://github.com/coilyco-flight-deck/reddit-mcp) - Read-only MCP for private Reddit feeds and public subreddit RSS.
- [`coilyco-flight-deck/scoop-bucket`](https://github.com/coilyco-flight-deck/scoop-bucket) - Scoop bucket for Windows binaries published by coilyco-flight-deck.
- [`coilyco-flight-deck/ward`](https://github.com/coilyco-flight-deck/ward) - Governed execution layer for unattended coding agents in isolated repository workflows.
- [`coilyco-flight-deck/ward-mcp`](https://github.com/coilyco-flight-deck/ward-mcp) - MCP runtime that turns cli-guard policy files into guarded streamable HTTP services and container images.

## Tags → repos

- [`ai-agents`](https://github.com/topics/ai-agents) - [`coilyco-flight-deck/.github`](https://github.com/coilyco-flight-deck/.github), [`coilyco-flight-deck/agent-compose`](https://github.com/coilyco-flight-deck/agent-compose), [`coilyco-flight-deck/agent-proxy`](https://github.com/coilyco-flight-deck/agent-proxy), [`coilyco-flight-deck/agentic-os`](https://github.com/coilyco-flight-deck/agentic-os), [`coilyco-flight-deck/ward`](https://github.com/coilyco-flight-deck/ward)
- [`ansible`](https://github.com/topics/ansible) - [`coilyco-flight-deck/infrastructure`](https://github.com/coilyco-flight-deck/infrastructure)
- [`automation`](https://github.com/topics/automation) - [`coilyco-flight-deck/agent-compose`](https://github.com/coilyco-flight-deck/agent-compose), [`coilyco-flight-deck/agentic-os`](https://github.com/coilyco-flight-deck/agentic-os), [`coilyco-flight-deck/cli-guard`](https://github.com/coilyco-flight-deck/cli-guard), [`coilyco-flight-deck/homebrew-tap`](https://github.com/coilyco-flight-deck/homebrew-tap), [`coilyco-flight-deck/scoop-bucket`](https://github.com/coilyco-flight-deck/scoop-bucket), [`coilyco-flight-deck/ward`](https://github.com/coilyco-flight-deck/ward), [`coilyco-flight-deck/ward-mcp`](https://github.com/coilyco-flight-deck/ward-mcp)
- [`bluesky`](https://github.com/topics/bluesky) - [`coilyco-flight-deck/bluesky-mcp`](https://github.com/coilyco-flight-deck/bluesky-mcp)
- [`command-line`](https://github.com/topics/command-line) - [`coilyco-flight-deck/cli-guard`](https://github.com/coilyco-flight-deck/cli-guard)
- [`devops`](https://github.com/topics/devops) - [`coilyco-flight-deck/.github`](https://github.com/coilyco-flight-deck/.github), [`coilyco-flight-deck/cli-guard`](https://github.com/coilyco-flight-deck/cli-guard), [`coilyco-flight-deck/homebrew-tap`](https://github.com/coilyco-flight-deck/homebrew-tap), [`coilyco-flight-deck/scoop-bucket`](https://github.com/coilyco-flight-deck/scoop-bucket), [`coilyco-flight-deck/ward`](https://github.com/coilyco-flight-deck/ward)
- [`dotfiles`](https://github.com/topics/dotfiles) - [`coilyco-flight-deck/agentic-os`](https://github.com/coilyco-flight-deck/agentic-os)
- [`github-profile`](https://github.com/topics/github-profile) - [`coilyco-flight-deck/.github`](https://github.com/coilyco-flight-deck/.github)
- [`helm`](https://github.com/topics/helm) - [`coilyco-flight-deck/lunch-money-k8s`](https://github.com/coilyco-flight-deck/lunch-money-k8s)
- [`homelab`](https://github.com/topics/homelab) - [`coilyco-flight-deck/infrastructure`](https://github.com/coilyco-flight-deck/infrastructure)
- [`homebrew`](https://github.com/topics/homebrew) - [`coilyco-flight-deck/homebrew-tap`](https://github.com/coilyco-flight-deck/homebrew-tap)
- [`infrastructure-as-code`](https://github.com/topics/infrastructure-as-code) - [`coilyco-flight-deck/infrastructure`](https://github.com/coilyco-flight-deck/infrastructure)
- [`kubernetes`](https://github.com/topics/kubernetes) - [`coilyco-flight-deck/infrastructure`](https://github.com/coilyco-flight-deck/infrastructure), [`coilyco-flight-deck/node-stats-mcp`](https://github.com/coilyco-flight-deck/node-stats-mcp)
- [`llm`](https://github.com/topics/llm) - [`coilyco-flight-deck/agent-compose`](https://github.com/coilyco-flight-deck/agent-compose), [`coilyco-flight-deck/agent-proxy`](https://github.com/coilyco-flight-deck/agent-proxy)
- [`mcp`](https://github.com/topics/mcp) - [`coilyco-flight-deck/agent-compose`](https://github.com/coilyco-flight-deck/agent-compose), [`coilyco-flight-deck/bluesky-mcp`](https://github.com/coilyco-flight-deck/bluesky-mcp), [`coilyco-flight-deck/lunch-money-k8s`](https://github.com/coilyco-flight-deck/lunch-money-k8s), [`coilyco-flight-deck/node-stats-mcp`](https://github.com/coilyco-flight-deck/node-stats-mcp), [`coilyco-flight-deck/reddit-mcp`](https://github.com/coilyco-flight-deck/reddit-mcp), [`coilyco-flight-deck/ward-mcp`](https://github.com/coilyco-flight-deck/ward-mcp)
- [`model-context-protocol`](https://github.com/topics/model-context-protocol) - [`coilyco-flight-deck/bluesky-mcp`](https://github.com/coilyco-flight-deck/bluesky-mcp), [`coilyco-flight-deck/lunch-money-k8s`](https://github.com/coilyco-flight-deck/lunch-money-k8s), [`coilyco-flight-deck/reddit-mcp`](https://github.com/coilyco-flight-deck/reddit-mcp), [`coilyco-flight-deck/ward-mcp`](https://github.com/coilyco-flight-deck/ward-mcp)
- [`observability`](https://github.com/topics/observability) - [`coilyco-flight-deck/.github`](https://github.com/coilyco-flight-deck/.github), [`coilyco-flight-deck/agent-proxy`](https://github.com/coilyco-flight-deck/agent-proxy), [`coilyco-flight-deck/node-stats-mcp`](https://github.com/coilyco-flight-deck/node-stats-mcp)
- [`opentelemetry`](https://github.com/topics/opentelemetry) - [`coilyco-flight-deck/agent-proxy`](https://github.com/coilyco-flight-deck/agent-proxy), [`coilyco-flight-deck/node-stats-mcp`](https://github.com/coilyco-flight-deck/node-stats-mcp)
- [`personal-finance`](https://github.com/topics/personal-finance) - [`coilyco-flight-deck/lunch-money-k8s`](https://github.com/coilyco-flight-deck/lunch-money-k8s)
- [`reddit`](https://github.com/topics/reddit) - [`coilyco-flight-deck/reddit-mcp`](https://github.com/coilyco-flight-deck/reddit-mcp)
- [`rss`](https://github.com/topics/rss) - [`coilyco-flight-deck/reddit-mcp`](https://github.com/coilyco-flight-deck/reddit-mcp)
- [`scoop`](https://github.com/topics/scoop) - [`coilyco-flight-deck/scoop-bucket`](https://github.com/coilyco-flight-deck/scoop-bucket)
- [`security`](https://github.com/topics/security) - [`coilyco-flight-deck/agentic-os`](https://github.com/coilyco-flight-deck/agentic-os), [`coilyco-flight-deck/bluesky-mcp`](https://github.com/coilyco-flight-deck/bluesky-mcp), [`coilyco-flight-deck/cli-guard`](https://github.com/coilyco-flight-deck/cli-guard), [`coilyco-flight-deck/ward`](https://github.com/coilyco-flight-deck/ward), [`coilyco-flight-deck/ward-mcp`](https://github.com/coilyco-flight-deck/ward-mcp)

## Repos → tags

- [`coilyco-flight-deck/.github`](https://github.com/coilyco-flight-deck/.github) - [`ai-agents`](https://github.com/topics/ai-agents), [`devops`](https://github.com/topics/devops), [`github-profile`](https://github.com/topics/github-profile), [`observability`](https://github.com/topics/observability)
- [`coilyco-flight-deck/agent-compose`](https://github.com/coilyco-flight-deck/agent-compose) - [`ai-agents`](https://github.com/topics/ai-agents), [`automation`](https://github.com/topics/automation), [`llm`](https://github.com/topics/llm), [`mcp`](https://github.com/topics/mcp)
- [`coilyco-flight-deck/agent-proxy`](https://github.com/coilyco-flight-deck/agent-proxy) - [`ai-agents`](https://github.com/topics/ai-agents), [`llm`](https://github.com/topics/llm), [`observability`](https://github.com/topics/observability), [`opentelemetry`](https://github.com/topics/opentelemetry)
- [`coilyco-flight-deck/agentic-os`](https://github.com/coilyco-flight-deck/agentic-os) - [`ai-agents`](https://github.com/topics/ai-agents), [`automation`](https://github.com/topics/automation), [`dotfiles`](https://github.com/topics/dotfiles), [`security`](https://github.com/topics/security)
- [`coilyco-flight-deck/bluesky-mcp`](https://github.com/coilyco-flight-deck/bluesky-mcp) - [`bluesky`](https://github.com/topics/bluesky), [`mcp`](https://github.com/topics/mcp), [`model-context-protocol`](https://github.com/topics/model-context-protocol), [`security`](https://github.com/topics/security)
- [`coilyco-flight-deck/cli-guard`](https://github.com/coilyco-flight-deck/cli-guard) - [`automation`](https://github.com/topics/automation), [`command-line`](https://github.com/topics/command-line), [`devops`](https://github.com/topics/devops), [`security`](https://github.com/topics/security)
- [`coilyco-flight-deck/homebrew-tap`](https://github.com/coilyco-flight-deck/homebrew-tap) - [`automation`](https://github.com/topics/automation), [`devops`](https://github.com/topics/devops), [`homebrew`](https://github.com/topics/homebrew)
- [`coilyco-flight-deck/infrastructure`](https://github.com/coilyco-flight-deck/infrastructure) - [`ansible`](https://github.com/topics/ansible), [`homelab`](https://github.com/topics/homelab), [`infrastructure-as-code`](https://github.com/topics/infrastructure-as-code), [`kubernetes`](https://github.com/topics/kubernetes)
- [`coilyco-flight-deck/lunch-money-k8s`](https://github.com/coilyco-flight-deck/lunch-money-k8s) - [`helm`](https://github.com/topics/helm), [`mcp`](https://github.com/topics/mcp), [`model-context-protocol`](https://github.com/topics/model-context-protocol), [`personal-finance`](https://github.com/topics/personal-finance)
- [`coilyco-flight-deck/node-stats-mcp`](https://github.com/coilyco-flight-deck/node-stats-mcp) - [`kubernetes`](https://github.com/topics/kubernetes), [`mcp`](https://github.com/topics/mcp), [`observability`](https://github.com/topics/observability), [`opentelemetry`](https://github.com/topics/opentelemetry)
- [`coilyco-flight-deck/reddit-mcp`](https://github.com/coilyco-flight-deck/reddit-mcp) - [`mcp`](https://github.com/topics/mcp), [`model-context-protocol`](https://github.com/topics/model-context-protocol), [`reddit`](https://github.com/topics/reddit), [`rss`](https://github.com/topics/rss)
- [`coilyco-flight-deck/scoop-bucket`](https://github.com/coilyco-flight-deck/scoop-bucket) - [`automation`](https://github.com/topics/automation), [`devops`](https://github.com/topics/devops), [`scoop`](https://github.com/topics/scoop)
- [`coilyco-flight-deck/ward`](https://github.com/coilyco-flight-deck/ward) - [`ai-agents`](https://github.com/topics/ai-agents), [`automation`](https://github.com/topics/automation), [`devops`](https://github.com/topics/devops), [`security`](https://github.com/topics/security)
- [`coilyco-flight-deck/ward-mcp`](https://github.com/coilyco-flight-deck/ward-mcp) - [`automation`](https://github.com/topics/automation), [`mcp`](https://github.com/topics/mcp), [`model-context-protocol`](https://github.com/topics/model-context-protocol), [`security`](https://github.com/topics/security)

## Elsewhere

- Personal site: [coilysiren.me](https://coilysiren.me)
- Operational back-office: [coilyco-bridge](https://github.com/coilyco-bridge) (canonical at [Forgejo](https://forgejo.coilysiren.me/coilyco-bridge))
