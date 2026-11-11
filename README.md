# AI Engineering Handbook

A structured, in-depth guide to AI engineering, from foundations to production. It is written for experienced software engineers moving into AI engineering, Forward Deployed Engineer (FDE) and AI solution architect roles, and it doubles as interview preparation.

Each chapter explains a concept from scratch, shows where it is used in industry, and ends with interview questions, a scenario exercise and revision points.

## How to use this handbook

- **Read in order the first time.** Chapters are numbered in learning order, and each one relies only on ideas from earlier chapters.
- **Every chapter follows the same short template:** the concept in interview language, analogies, diagrams, industry use cases, common misconceptions, interview questions, a scenario exercise, key takeaways and further reading. A chapter takes about 10-20 minutes.
- **Practise out loud.** Each interview question comes with a full model answer written the way you would say it. Cover the answer, say yours aloud, then compare.
- **Attempt the scenario exercise before opening the answer.** The model answer is collapsed on purpose.
- **Revise from the key takeaways.** The night before an interview, read only the "Key takeaways" section of each chapter.
- **Check dates on fast-moving facts.** Model names, context sizes, prices and protocol versions change quickly. They are marked "(as of Mon YYYY)" and linked to a source. Treat older marks with suspicion.

## Table of contents

### Part 1: Foundations

1. [Introduction to AI](chapters/01-introduction-to-ai/README.md): what AI, machine learning, deep learning and generative AI are, and what AI engineering adds.
2. [How machines learn](chapters/02-how-machines-learn/README.md): supervised, unsupervised and reinforcement learning, gradient descent, over- and underfitting, neural networks.

### Part 2: How LLMs work

3. [Tokens and embeddings](chapters/03-tokens-and-embeddings/README.md): how text becomes tokens, token IDs and vectors, and why meaning lives in distance.
4. [Transformers and attention](chapters/04-transformers-and-attention/README.md): self-attention, the layer stack, and why training parallelises.
5. [Training LLMs](chapters/05-training-llms/README.md): pre-training, scale, parameters, base vs instruct vs reasoning models, SFT and RLHF.
6. [Inference and generation](chapters/06-inference-and-generation/README.md): stateless calls, sampling controls, streaming, structured output, and why models hallucinate.
7. [Context windows and context engineering](chapters/07-context-windows-and-context-engineering/README.md): what fits, what it costs, and how to fill the window deliberately.
8. [The model landscape](chapters/08-the-model-landscape/README.md): frontier, open-weight and small models, multimodal and diffusion models, and how to choose.

### Part 3: Shaping model behaviour

9. [Prompt engineering](chapters/09-prompt-engineering/README.md): prompt anatomy, few-shot examples, chaining, structured outputs, versioning and prompt caching.
10. [Fine-tuning and distillation](chapters/10-fine-tuning-and-distillation/README.md): when to adapt weights, LoRA and QLoRA, quantisation, distillation and small models.

### Part 4: Retrieval-Augmented Generation (RAG)

11. [RAG fundamentals](chapters/11-rag-fundamentals/README.md): why RAG exists, parametric vs non-parametric memory, and the two pipelines.
12. [Ingestion and chunking](chapters/12-ingestion-and-chunking/README.md): parsing documents, chunking strategies, overlap, parent-child and metadata.
13. [Vector search and databases](chapters/13-vector-search-and-databases/README.md): approximate nearest neighbour search, BM25, dense and hybrid retrieval, and scaling an index.
14. [Improving retrieval](chapters/14-improving-retrieval/README.md): query transformation, reranking, context expansion and agentic RAG.
15. [Enterprise RAG](chapters/15-enterprise-rag/README.md): permission-aware retrieval, citations, conflicting documents and scale.
16. [RAG vs fine-tuning vs long context](chapters/16-rag-vs-fine-tuning-vs-long-context/README.md): a decision framework you can defend.

### Part 5: Agents

17. [From LLM calls to agents](chapters/17-from-llm-calls-to-agents/README.md): the agent loop, ReAct, agent types, and workflow vs agent.
18. [Tool calling](chapters/18-tool-calling/README.md): tool schemas, who executes what, tool design, errors and permissions.
19. [Agent protocols: MCP and A2A](chapters/19-agent-protocols-mcp-and-a2a/README.md): standard connections to tools, data and other agents.
20. [Agent memory and state](chapters/20-agent-memory-and-state/README.md): short-term, long-term and episodic memory, and keeping memory fresh.
21. [Orchestration and harnesses](chapters/21-orchestration-and-harnesses/README.md): control loops, frameworks, checkpoints and human-in-the-loop gates.
22. [Multi-agent systems](chapters/22-multi-agent-systems/README.md): supervisors and workers, error propagation, cost and tracing.
23. [Agent-user interaction](chapters/23-agent-user-interaction/README.md): streaming, steerable agents, AG-UI and voice agents.
24. [Agent reliability and learning](chapters/24-agent-reliability-and-learning/README.md): loops, wrong tool choices, compounding error and learning from production.

### Part 6: Quality and safety

25. [Evaluation fundamentals](chapters/25-evaluation-fundamentals/README.md): golden datasets, LLM-as-judge, benchmarks and why high scores can still disappoint users.
26. [Evaluating RAG and agents](chapters/26-evaluating-rag-and-agents/README.md): retrieval and generation metrics, agent trajectories and measuring a reranker.
27. [Hallucination and grounding](chapters/27-hallucination-and-grounding/README.md): layers that reduce hallucination, abstention and confidence.
28. [Guardrails and AI security](chapters/28-guardrails-and-ai-security/README.md): prompt injection, jailbreaks, least privilege and PII redaction.
29. [Privacy, governance and compliance](chapters/29-privacy-governance-and-compliance/README.md): data retention, identity, audit trails and regulation.

### Part 7: Production (LLMOps)

30. [Cost, latency and caching](chapters/30-cost-latency-and-caching/README.md): cutting cost, time to first token, prompt and semantic caching.
31. [Observability and LLMOps](chapters/31-observability-and-llmops/README.md): tracing, prompt management, safe rollouts and feedback loops.
32. [Self-hosting open-weight models](chapters/32-self-hosting-open-weight-models/README.md): local and private deployment, batching, KV cache and cost estimates.
33. [Reliability, scaling and streaming](chapters/33-reliability-scaling-and-streaming/README.md): retries, fallbacks, SSE streaming and surviving 100x traffic.
34. [LLM gateways and routing](chapters/34-llm-gateways-and-routing/README.md): one front door for many teams, model routers and rate limits.
35. [Cloud reference architectures and multi-tenancy](chapters/35-cloud-reference-architectures-and-multi-tenancy/README.md): AWS, Azure and Google Cloud patterns and tenant isolation.

### Part 8: Delivery and interviews

36. [Forward deployed engineering](chapters/36-forward-deployed-engineering/README.md): discovery, scoping, proof of concept to production, and talking to clients.
37. [AI system design](chapters/37-ai-system-design/README.md): a repeatable method for design questions, with worked examples.
38. [Interview playbook](chapters/38-interview-playbook/README.md): answer structure, common traps and a rapid-fire revision sheet.
