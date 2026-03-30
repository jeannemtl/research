# Research Pipeline Results

Two-agent research pipeline: Hermes 1 (Mac mini supervisor) dispatches tasks to Hermes 2 (RunPod GPU worker).

## Branches

Each research task lives on its own branch. Main serves as the index.

| Branch | Topic | Date | Status |
|--------|-------|------|--------|
| — | — | — | No research tasks yet |

## How it works

1. Research task dispatched to RunPod GPU worker
2. Worker runs Hermes Agent to investigate
3. Results pulled back and reviewed by supervisor
4. Results committed to a new branch
5. Summary delivered to Telegram + Discord
6. Models (if any) pushed to HuggingFace: [prompterminal](https://huggingface.co/prompterminal)

## Structure (per branch)

```
results.md          — main research findings
worker_log.txt      — raw Hermes worker output
*.py                — any scripts produced
models/             — model files (if any, also pushed to HF)
```
