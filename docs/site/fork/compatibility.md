# Tracking and sync policy

> **Maintained fork.** This is a ForgeGuard-maintained downstream fork of [`vllm-project/vllm`](https://github.com/vllm-project/vllm). vLLM is upstream-owned and upstream-developed. ForgeGuard-specific documentation is **not** endorsed, supported, or reviewed by the upstream project.

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

## What this fork is, and is not

This fork's `main` branch mirrors the upstream default branch as of the base commit above. It
is **not** a curated release channel, and ForgeGuard does not test, build, or distribute it.

The base is an untagged development commit (`49f31d7cee42`) of the upstream default branch — **not an upstream release**.

For anything you intend to run, use an upstream release:
<https://github.com/vllm-project/vllm/releases>

## Product notes

Properties of vLLM itself, stated so readers understand the project. ForgeGuard has
verified none of them by execution:

- vLLM exposes an OpenAI-compatible server; the official image entrypoint is `vllm serve`.
- Models requiring `--trust-remote-code` execute arbitrary code from the model repository, and Hugging Face model revisions are mutable unless pinned with `--revision`.

For authoritative and current requirements, use upstream: <https://docs.vllm.ai/>

## Sync cadence

ForgeGuard refreshes the fork from upstream on a best-effort basis, following
[`docs/maintainers/upstream-sync/sync-checklist.md`](../../maintainers/upstream-sync/sync-checklist.md).
There is no SLA. When the fork is refreshed, `FORK_UPSTREAM_BASE` is updated to the new base commit.

## Relationship to upstream distribution

Upstream's own distribution is the only distribution. ForgeGuard does not publish an alternative and
does not suggest that upstream packaging is deficient.
