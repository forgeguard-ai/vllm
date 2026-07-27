# Security policy — ForgeGuard fork

This page covers the **ForgeGuard fork** of
[`vllm-project/vllm`](https://github.com/vllm-project/vllm). It does not replace the upstream
project's own security policy.

## Where to report

| Issue | Report to |
|---|---|
| Vulnerability in vLLM itself | Upstream — see [the upstream security policy](../../../SECURITY.md) shipped in this repository |
| A problem with ForgeGuard documentation, such as an incorrect fork base or misleading security guidance | ForgeGuard — privately, see below |

**Never open a public issue for a suspected vulnerability.**

Report ForgeGuard documentation issues privately through
[GitHub private vulnerability reporting](https://github.com/forgeguard-ai/vllm/security/advisories/new).

## Scope

ForgeGuard publishes **no container image, package, or release** for this repository, so there is no
ForgeGuard supply chain to attack and no ForgeGuard artifact to verify. The surface ForgeGuard owns
is limited to:

- the accuracy of the recorded base in [`FORK_UPSTREAM_BASE`](../../../FORK_UPSTREAM_BASE),
- the documentation-validation workflow under `.github/workflows/`.

Everything about running vLLM — its dependencies, its images, its runtime security — is
upstream's, and should be evaluated against upstream's published artifacts.

## Deployment security notes

- vLLM exposes an OpenAI-compatible server; the official image entrypoint is `vllm serve`.
- Models requiring `--trust-remote-code` execute arbitrary code from the model repository, and Hugging Face model revisions are mutable unless pinned with `--revision`.

Verify these against upstream documentation before relying on them.
