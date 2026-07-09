# Aidan Joneleit

ML engineering across the full stack — training, RL post-training, and inference systems.
EECS + Business @ UC Berkeley (M.E.T. '28).

Currently: machine learning engineer at **TriasBio**, fine-tuning RNA language models for
personalized therapeutics. Previously: built RL environments and agent evals (**OpenAI**,
contract) and on-device LLM serving on Snapdragon with ONNX/QNN (**Qualcomm**, contract).

## Featured work

### [kestrel](https://github.com/joneleit/kestrel) — an LLM inference engine from scratch

Paged KV cache with prefix caching, continuous batching with chunked prefill and
preemption, speculative decoding, INT8 weight-only quantization, a Triton
paged-attention decode kernel, and an OpenAI-compatible server with Prometheus
metrics. No vLLM, no TGI — the point is owning every layer between an HTTP
request and the kernel.

- Core invariant enforced by tests: paged, batched, cache-reusing decoding is
  **token-for-token identical** to naive dense decoding — including under forced
  preemption and prefix-cache reuse
- Speculative decoding verified against the exactness guarantee (greedy identity +
  distributional equality), not eyeballed outputs
- Ships with Terraform for GPU spot serving, an EKS manifest that autoscales on
  KV-cache pressure instead of CPU, and a Grafana dashboard for TTFT/throughput/KV
- `pytest`: 41 passed (3 GPU kernel tests run on the deploy box)

### [loom](https://github.com/joneleit/loom) — training a small LLM end to end

Byte-level BPE → packed-corpus pretraining → prompt-masked SFT → **GRPO implemented
from the math up** (group-relative advantages, PPO-clip surrogate, k3 KL to a frozen
reference — no TRL) → eval harness with unbiased pass@k and contamination gates.

- The whole pipeline actually runs and is committed with its metrics: held-out
  accuracy **3% → 20% → 26%** across pretrain → SFT → GRPO on a
  verifiable-reward task with train/eval disjoint by construction
- DDP/FSDP trainer with atomic checkpoints: interrupt-and-resume is **bitwise
  identical** to an uninterrupted run (unit-tested) — built for spot instances
- Documented failure modes I hit and fixed: GRPO's zero-variance cold start,
  contamination false positives from substring matching, torn checkpoints from
  non-atomic saves

Both repos carry a `DESIGN.md` (decisions + tradeoffs) and a `ROADMAP.md` of open
exercises I'm working through — benchmarks vs. vLLM and a 20M-param TinyStories
run are next.

## Elsewhere

- Founded **PokePulse**, a Python e-commerce platform with dynamic repricing
  (~500 SKUs, ~$21K/mo profit) — seven years of keeping production software alive
- Published research on stochastic modeling for cryptocurrency valuation (ICFTBA 2024);
  led a DeFi platform build with ~3,000 transactions in open beta
- Eagle Scout; led a 176-mile Philmont expedition. I still disappear into the
  backcountry when the training runs are stable.

## Contact

[joneleit@berkeley.edu](mailto:joneleit@berkeley.edu) ·
[LinkedIn](https://www.linkedin.com/in/aidanjoneleit)
