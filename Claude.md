# AI Engineering Handbook: project rules

## Purpose
A structured, in-depth learning handbook on AI engineering, from foundations to production,
written for Brijesh (senior software engineer, 15+ years, moving into AI engineering /
Forward Deployed Engineer / AI solution architect roles). It replaces scattered notes and
doubles as interview preparation. It will be public on GitHub.

## Source material
- `sources/` holds Brijesh's own notes (Notion PDF exports) and an interview answer bank.
- Use them as the starting point for content and coverage, but do not copy them blindly:
  reorganise, deepen, and correct them.
- Known errors in the notes that must NOT be carried over:
  - Tokenisation and embedding are separate steps (text → tokens → token IDs → vectors).
  - ANN in vector search = approximate nearest neighbour, not artificial neural network.
  - Bi-encoders do first-stage retrieval; cross-encoders and ColBERT-style late interaction do reranking.
  - Small/mini models often have large context windows (128K+ tokens), not 2,000–4,000 words.
  - "Most LLMs handle ~32K tokens" is outdated.
  - Quantisation commonly goes to 8-bit and 4-bit, not just 32→16-bit.
  - Distillation trains a small model to imitate a large model's outputs.
  - MCP does not "understand the query"; the LLM decides, MCP is the standard connection to tools/data.
  - Remove unverified figures (e.g. GPT-4 parameter counts, model task-duration claims).

## Repository structure
- `README.md`: the handbook's table of contents, grouped by part, linking to every chapter, plus a short "how to use this handbook" section.
- `chapters/NN-chapter-slug/README.md`: one folder per chapter, numbered in learning order.
- `chapters/NN-chapter-slug/examples/`: optional small Python examples for that chapter.
- `sources/`: Brijesh's raw notes (input only; never edit).

## Learning order (each chapter may only rely on concepts from earlier chapters)
Part 1 Foundations · Part 2 How LLMs work · Part 3 Shaping model behaviour · Part 4 RAG ·
Part 5 Agents · Part 6 Quality and safety · Part 7 Production (LLMOps) · Part 8 Delivery and interviews.
The table of contents in README.md is the source of truth for chapter names and order.

## Chapter template (use these sections, in this order)
1. **Why it matters**: 2–3 lines on where this shows up in real systems.
2. **The concept, from scratch**: plain English first, then the precise technical version. Define every term the first time it appears.
3. **Analogies across industries**: see the analogy rule below.
4. **Diagram**: in Mermaid (GitHub renders it). At least one per chapter where a picture helps.
5. **How it's used in industry**: 2–4 short real-world use cases from different industries.
6. **Common misconceptions**: what people get wrong, including interview traps.
7. **Python example** (only where it genuinely helps understanding): small, runnable, minimal dependencies, explained line by line. Put longer ones in `examples/`.
8. **Interview questions**: easiest first. Each with a model answer in this format:
   - **Say first:** the 1–2 sentence answer to open with.
   - **Then cover:** the key points, in speaking order.
   - **Architect angle:** the trade-off, cost, governance or client point that lifts the answer.
   - **Trap:** the common wrong answer or likely follow-up.
9. **Scenario exercise**: one short client-style case with incomplete information, to answer from memory. Put a model answer inside a collapsed `<details>` block so it can be attempted first.
10. **Key takeaways**: 3–5 one-line points for revision.
11. **Further reading**: 2–5 credible sources (official docs, papers, vendor engineering blogs).

## Analogy rule
- Do not default to banking. Rotate across industries: banking, insurance, healthcare,
  e-commerce, retail, logistics, telecom, manufacturing, travel, government/public sector.
- Each chapter uses at least two different industries across its analogies and use cases.
- Analogies must be accurate to how that industry actually works; keep them concrete
  (e.g. "a hospital triage nurse routing patients" for a model router).

## Accuracy rules
- Correctness matters more than coverage. This is used in interviews.
- For anything that changes fast (model names, context sizes, prices, protocol versions such as MCP and A2A,
  framework features, cloud service names), verify with a web search before writing and link the source.
- Mark time-sensitive facts with "(as of Mon YYYY)".
- If something is uncertain or disputed, say so plainly rather than stating it as fact.
- Never invent statistics, benchmarks or quotes.

## Writing style
- Plain, direct English. Short paragraphs. Explain like a senior engineer teaching a smart colleague who is new to AI.
- Prose for explanations; lists only where items are genuinely parallel. No filler, no hype, no emojis.
- Link related chapters inline (relative links) the first time a concept from another chapter appears.
- Each chapter should take about 20–40 minutes to read.

## Workflow
- Work one part at a time. Before writing a part, propose the chapter outlines and wait for approval.
- After writing a chapter, update README.md and check that all links resolve.
- Never edit files in `sources/`.
- Do not commit or push; Brijesh reviews and commits himself.