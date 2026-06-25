# Engrammic Research

## Before intelligence can be trusted, it must learn to doubt.

AI systems retrieve, generate, and confidently hallucinate. When they are wrong, they do not notice - nothing in how they work tracks the difference between what was observed and what was concluded. There is no mechanism for doubt, no architecture for uncertainty, no way to ask "why do I believe this?" and receive a real answer.

This is the problem that is not being solved. We are racing to make AI more capable, but capability without epistemics is just a more eloquent way to be wrong.

Consider why you trust people. It is not because they are always right. It is because when they are wrong, they notice. They update. They hold their beliefs loosely enough to revise them. They can tell you why they believe what they believe, and what evidence would change their mind.

This is not a feature bolted onto human intelligence. This is the shape intelligence takes when it is honest with itself.

## The Open Problem

We believe aligned, trustworthy AI will not come from scaling parameters alone. It will come from systems that think epistemically: systems that know what they know, why they believe it, and when to update. Systems that distinguish between observation and conclusion, between confident and uncertain, between current and outdated.

Concretely, we need AI that can:

- **Hold doubt** - distinguish observations from claims from verified facts from synthesized beliefs
- **Trace provenance** - follow any belief back to the observations that ground it
- **Revise coherently** - update dependent beliefs when underlying evidence shifts
- **Coordinate truthfully** - maintain shared understanding across agents without contradiction

No existing system does all four. This repository contains our research toward solving this problem. We publish openly because the problem is too important to solve alone.

## Our Approach

We treat agent memory as applied epistemology: stratified belief types with distinct evidence requirements, write-time coherence enforcement, and formal belief revision that preserves audit trails.

The papers here formalize this approach. We invite the research community to critique, extend, challenge, and build upon this work.

## Papers

**[Beyond Retrieval: Layered Epistemic Agent Protocol for Coherent Agent Memory](papers/whitepaper-beyond-retrieval.tex)**

The technical paper. Introduces LeAP with stratified epistemic types, warrant functions, coherence invariants, and AGM-compliant belief revision. Presents CITE, a four-layer architecture with write-time coherence enforcement.

**[From Memory to Epistemics](papers/whitepaper-memory-to-epistemics.tex)**

The foundational argument. Convergent evidence from information theory, optimization, interpretability, distributed systems, and neuroscience that epistemic state must live outside the models doing inference.

## Contributing

We welcome:

- **Critique** - holes in arguments, missing prior work, unsupported claims
- **Extensions** - new theorems, connections to other frameworks
- **Benchmarks** - evaluation methodologies that measure what matters
- **Implementations** - architectures satisfying the same axioms

See [CONTRIBUTING.md](CONTRIBUTING.md).

## Building

```bash
cd papers
pdflatex whitepaper-beyond-retrieval.tex
bibtex whitepaper-beyond-retrieval
pdflatex whitepaper-beyond-retrieval.tex
pdflatex whitepaper-beyond-retrieval.tex
```

## Related

- [Engrammic](https://github.com/engrammic-ai/engrammic) - Reference implementation
- [engrammic-primitives](https://pypi.org/project/engrammic-primitives/) - Schema and types

## License

CC BY-SA 4.0
