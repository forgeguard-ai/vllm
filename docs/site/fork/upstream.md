# Upstream project and attribution

> **Maintained fork.** This is a ForgeGuard-maintained downstream fork of [`vllm-project/vllm`](https://github.com/vllm-project/vllm). vLLM is upstream-owned and upstream-developed. ForgeGuard-specific documentation is **not** endorsed, supported, or reviewed by the upstream project.

## The upstream project

vLLM is developed and owned by [`vllm-project/vllm`](https://github.com/vllm-project/vllm).

- Upstream repository: <https://github.com/vllm-project/vllm>
- Upstream documentation: <https://docs.vllm.ai/>
- Upstream releases: <https://github.com/vllm-project/vllm/releases>

The upstream README from this fork's base commit is preserved verbatim at
[`upstream-readme.md`](./upstream-readme.md).

## Fork base

| Field | Value |
|---|---|
| Upstream repository | [`vllm-project/vllm`](https://github.com/vllm-project/vllm) |
| Fork default branch | `main` |
| Base commit | `49f31d7cee425a6d38f8c5bc76877986daf832ed` |
| Tag at that commit | _none — untagged development commit_ |
| Upstream license | Apache-2.0 |
| Documented on | 2026-07-27 |
| ForgeGuard artifacts | **none published** |

The machine-readable source of truth is [`FORK_UPSTREAM_BASE`](../../../FORK_UPSTREAM_BASE),
validated in CI against `.forgeguard/schemas/fork-upstream-base.schema.json`.

**This fork is not a release channel.** Its base is
an untagged development commit (`49f31d7cee42`) of the upstream default branch — **not an upstream release**. For a supported version, use an upstream release.

## License and attribution

vLLM is distributed under the **Apache-2.0**. Apache License 2.0, verified in the tagged source tree.

The upstream `LICENSE` file, copyright notices, and any `NOTICE` material are preserved unchanged.
ForgeGuard documentation does not relicense upstream code.

ForgeGuard claims no ownership of vLLM, its name, its logo, or its trademarks. Nothing in
this fork implies that the upstream project created, endorses, sponsors, or supports it.

## Support boundary

| Area | Owner |
|---|---|
| ForgeGuard documentation under `docs/site/` | ForgeGuard |
| The recorded fork base and sync cadence | ForgeGuard |
| vLLM features, correctness, performance, model support | Upstream |
| Security vulnerabilities in vLLM itself | Upstream, per upstream policy |
| Distribution of runnable artifacts | **Upstream only.** ForgeGuard publishes none. |
