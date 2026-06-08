# PlatformKit OSS

**PlatformKit** is a modular SaaS framework in Go for building governed, composable applications — identity, tenancy, admin, content, audit, notifications, and deployment paths, without rebuilding the same substrate every time.

Built by [Septagon](https://septagon.dev). Licensed under Apache 2.0.

## Start here

| If you want to… | go to |
|-----------------|-------|
| Follow the 5-minute quickstart tutorial | [`pk-docs`](https://github.com/septagon-oss/pk-docs) — architecture, ADRs, tutorials |
| Run a complete SaaS app in one command | [`pk-apps`](https://github.com/septagon-oss/pk-apps) — starter-saas |
| Use the core building blocks | [`pk-core`](https://github.com/septagon-oss/pk-core) — module system, authz, entities, security |
| Browse the reference modules | [`pk-modules`](https://github.com/septagon-oss/pk-modules) — tenant, user, auth, api key, content, notification, audit, admin, health |
| Use the CLI and scaffold tools | [`pk-tools`](https://github.com/septagon-oss/pk-tools) — doctor, verify, explain |
| Ask questions or discuss | [Community discussions](https://github.com/septagon-dev/platformkit-community/discussions) |

```
go get github.com/septagon-oss/pk-core@latest
```

## Quickstart

```bash
go install github.com/septagon-oss/pk-apps/apps/starter-saas@latest
starter-saas
# → http://localhost:8080 — a complete SaaS app with auth, admin, and nine reference modules
```

Full tutorial → [pk-docs starter-saas guide](https://github.com/septagon-oss/pk-docs)

## Repository map (by dependency order)

| Layer | Repo | Role |
|-------|------|------|
| Core | [`pk-core`](https://github.com/septagon-oss/pk-core) | Module system, authz, entities, security, observability, resilience |
| Core | [`pk-registry`](https://github.com/septagon-oss/pk-registry) | Generic `Registry[T]` — zero-dependency, thread-safe |
| Core | [`pk-shared`](https://github.com/septagon-oss/pk-shared) | Shared vocabulary — flow definitions, state machines, composition |
| Core | [`pk-design`](https://github.com/septagon-oss/pk-design) | Design tokens, themes, component contracts |
| Runtime | [`pk-runtime`](https://github.com/septagon-oss/pk-runtime) | HTTP, health checks, request context, host composition |
| Modules | [`pk-modules`](https://github.com/septagon-oss/pk-modules) | Reference modules — tenant, user, auth, api key, content, notification, audit, admin, health |
| Apps | [`pk-apps`](https://github.com/septagon-oss/pk-apps) | Runnable compositions — starter-saas, examples |
| Tools | [`pk-tools`](https://github.com/septagon-oss/pk-tools) | CLI, scaffold, developer workflows |
| Client | [`pk-client`](https://github.com/septagon-oss/pk-client) | HTTP client — CRUD, bulk, typed envelopes |
| Test | [`pk-testkit`](https://github.com/septagon-oss/pk-testkit) | Conformance, flow, and API test contracts |
| Deploy | [`pk-deploy`](https://github.com/septagon-oss/pk-deploy) | Deployment kernel — plans, workers, evidence |
| Docs | [`pk-docs`](https://github.com/septagon-oss/pk-docs) | Architecture, ADRs, requirements, tutorials |
| UI | [`platformkit-ui`](https://github.com/septagon-oss/platformkit-ui) | UI contracts and accessibility helpers |

## Open-core model

The `septagon-oss` repos are the public upstream — stable, provider-neutral, Apache 2.0.
Pro modules (including billing and enterprise auth), cloud integrations, and enterprise
adapters live in companion repos under a separate organisation.

Core contracts stay provider-neutral. Databases, queues, cloud SDKs, and
business-specific flows belong in modules, apps, or Pro extensions.

## Community

- **Discussions** (hosted under our sister org): [septagon-dev/platformkit-community](https://github.com/septagon-dev/platformkit-community/discussions)
- **Bug reports:** open a GitHub issue in the relevant repo
- **Security:** report privately to `hello@septagon.dev`
- **License:** Apache 2.0 — see individual repo LICENSE files

Calm surface. Serious machinery underneath.
