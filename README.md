# Engrammic Research

## The Question

Can you trust an AI that cannot explain why it believes what it believes?

As AI agents become more autonomous, they accumulate beliefs over time. They learn from interactions, store observations, draw conclusions. But current systems have no structure for distinguishing a verified fact from a hallucination stored three sessions ago. No mechanism for propagating corrections. No way to answer "why do you believe that?" except by generating a plausible-sounding explanation.

This is not a retrieval problem. It is an epistemology problem.

## The Open Problem

We believe trustworthy AI requires agents that can:

- **Know what they know** - distinguish observations from claims from verified facts from synthesized beliefs
- **Know why they know it** - trace any belief back to its evidential roots
- **Revise coherently** - propagate corrections through dependent beliefs when facts change
- **Coordinate truthfully** - maintain shared understanding across multiple agents

No existing system does all four. We are publishing our research here because this problem is too important to solve alone.

## Our Approach

We propose treating agent memory as applied epistemology: stratified belief types with distinct evidence requirements, write-time coherence enforcement, and formal belief revision that preserves audit trails.

The papers in this repository formalize this approach and present an architecture for implementing it. We invite the broader research community to critique, extend, challenge, and build upon this work.

## Papers

**[Beyond Retrieval: Layered Epistemic Agent Protocol for Coherent Agent Memory](papers/whitepaper-beyond-retrieval.tex)**

The technical paper. Introduces LeAP, a framework with stratified epistemic types, warrant functions, coherence invariants, and AGM-compliant belief revision. Presents CITE, a four-layer architecture with write-time coherence enforcement. Includes formal definitions and proofs.

**[From Memory to Epistemics](papers/whitepaper-memory-to-epistemics.tex)**

The foundational argument. Convergent evidence from information theory, optimization, interpretability, distributed systems, and neuroscience that epistemic state must live outside the models doing inference.

## Contributing

We welcome:

- **Critique** - holes in our arguments, missing prior work, unsupported claims
- **Extensions** - new theorems, connections to other frameworks, alternative formalizations
- **Benchmarks** - evaluation methodologies that measure what matters
- **Implementations** - other architectures satisfying the same axioms

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

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
