# Vreko
[<img width="2172" height="724" alt="vreko-lockup" src="https://github.com/user-attachments/assets/3698fa6f-69ff-42f6-9152-faefc1001fd7" />](https://vreko.dev) — the intelligence layer for AI-native development.

## Product boundary

Read this first, because it determines what you will and will not find here.

**The Vreko core is proprietary.** The daemon, the intelligence engine, the pattern
store and the hosted service are not open source and are not published in this
organization.

**Selected interfaces are public** so that the surfaces you would integrate against can
be inspected, versioned and depended on:

| Surface | Repository | Distribution |
| --- | --- | --- |
| CLI | [`vreko-cli`](https://github.com/vreko-dev/vreko-cli) | [`@vreko/cli`](https://www.npmjs.com/package/@vreko/cli) |
| MCP server | [`mcp-server`](https://github.com/vreko-dev/mcp-server) | [`vreko-mcp-server`](https://www.npmjs.com/package/vreko-mcp-server) |
| VS Code extension | [`vscode`](https://github.com/vreko-dev/vscode) | **not currently installable** — the previous listing was unpublished and no Vreko-identified listing exists yet |

`vreko-cli` and `mcp-server` are **distribution and documentation surfaces**: they carry
the package manifest, changelog, license and docs that ship with each release. The
implementation is built from the private core, so you will not find it in those
repositories. This is deliberate, and stated there too.

## Also public

- [`ai-swarm`](https://github.com/vreko-dev/ai-swarm) — an audit-first, gate-controlled
  agent pipeline framework. Methodology and tooling, independent of the Vreko product.
- [`sopr-mcp`](https://github.com/vreko-dev/sopr-mcp) — **experimental.** A
  brand-neutral reference implementation of the Service-Oriented Protocol Router
  pattern for tool-heavy MCP servers. No performance benchmark is published for it;
  the repository says so explicitly.

## Install

```bash
npm install -g @vreko/cli
```

Then `vr --help`.

## External dependencies worth naming

Vreko consumes [**workspace.json**](https://workspacejson.dev), an independent
Apache-2.0 open standard for committed repository intelligence, maintained at
[`workspacejson`](https://github.com/workspacejson).

**Vreko does not own workspace.json.** It is a separate project with its own
organization, governance and release authority, and it is usable without Vreko.

## Archived

Superseded by the workspace.json standard, or retired in the rename from SnapBack to
Vreko. These remain readable for historical URLs only.

| Repository | Status |
| --- | --- |
| [`contracts`](https://github.com/vreko-dev/contracts) | Superseded by [`@workspacejson/spec`](https://www.npmjs.com/package/@workspacejson/spec) |
| [`config`](https://github.com/vreko-dev/config) | Deprecated |
| [`events`](https://github.com/vreko-dev/events) | Deprecated |
| [`sdk`](https://github.com/vreko-dev/sdk) | Deprecated |
| [`infrastructure`](https://github.com/vreko-dev/infrastructure) | Deprecated |

Their repository descriptions still read "package for SnapBack". GitHub does not allow
metadata edits on archived repositories, and unarchiving them purely to change a
description would misrepresent them as active.

## Links

- [vreko.dev](https://vreko.dev)
- [docs.vreko.dev](https://docs.vreko.dev)
- [Discord](https://discord.gg/B4BXeYkE2F)

## License

The public repositories in this organization are Apache-2.0 except
[`vscode`](https://github.com/vreko-dev/vscode) (GPL-3.0) and
[`sopr-mcp`](https://github.com/vreko-dev/sopr-mcp) (MIT). The Vreko core is
proprietary and is not covered by any of them.
