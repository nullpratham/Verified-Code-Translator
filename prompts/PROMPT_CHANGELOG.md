# Prompt Iteration Log — forked.exe

Date: 22 November 2026. This records prompt-design changes, not measured accuracy improvements. No comparative test runs are claimed.

| Version | What changed | Why | Evidence |
|---|---|---|---|
| V1 — Baseline | Basic C++→Python translation and short explanation. | Establish starting prompt. | No execution evidence. |
| V2 — Complexity-aware | Adds Big-O time/space, built-ins only, snake_case, avoiding copies, and explanations of typing, loops and memory. | Make complexity preservation explicit following M1 feedback. | More explicit requirements; no measured improvement claimed. |
| V3 — Verification-ready | Adds structured output, edge cases, behavioural-change disclosure and no unsupported execution claims. | Make output auditable and support a separate review stage. | Structured prompt; no measured improvement claimed. |

Three prompt versions are saved. The final workflow uses V3 for translation and a separate static verification prompt. Test execution and comparative prompt evaluation were not performed for this package.