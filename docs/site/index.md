# vLLM — ForgeGuard fork

> **Maintained fork.** This is a ForgeGuard-maintained downstream fork of [`vllm-project/vllm`](https://github.com/vllm-project/vllm). vLLM is upstream-owned and upstream-developed. ForgeGuard-specific documentation is **not** endorsed, supported, or reviewed by the upstream project.

ForgeGuard-maintained downstream fork of vLLM. **Documentation only — no ForgeGuard
build artifacts are published.**

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

This fork's branch adds ForgeGuard documentation on top of the default branch and modifies no
upstream source file. CI verifies that.

## Pages

- [Upstream project and attribution](./fork/upstream.md)
- [ForgeGuard changes (delta inventory)](./fork/forgeguard-changes.md)
- [Tracking and sync policy](./fork/compatibility.md)
- [Security policy](./fork/security.md)
- [Upstream README, preserved verbatim](./fork/upstream-readme.md)
- [Upstream sync runbook](../maintainers/upstream-sync/README.md)

## Installing the software

ForgeGuard publishes nothing. vLLM is installed from the upstream project, either as a Python package or via the official `vllm/vllm-openai` container image that upstream publishes. The tagged `docker/Dockerfile` at `v0.26.0` is the supported source build.

Authoritative product documentation: <https://docs.vllm.ai/>
