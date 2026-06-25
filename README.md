# Engrammic Research

## Why This Matters

Aligned AI needs to think in shapes humans recognize.

The alignment problem is often framed as getting AI to want the right things. But there is a deeper question: can AI reason in ways humans can follow, verify, and trust? An agent that reaches correct conclusions through opaque processes is not aligned - it is a black box that happens to agree with us today.

Human reasoning has structure. We distinguish observations from beliefs. We track why we believe things. We revise our views when evidence changes. We can explain our thinking to others who can then verify it.

We believe AI systems need the same epistemic structure - not because it makes them more capable, but because it makes alignment verifiable. An AI that externalizes its beliefs, grounds them in evidence, and revises them coherently is an AI whose reasoning humans can audit, challenge, and correct.

This is the foundation for agentic alignment: AI that thinks in the same shape as humans.

## The Open Problem

Current agent memory systems treat all stored information uniformly. A hallucination persists with the same standing as a verified fact. Contradictions accumulate. Corrections do not propagate. There is no answer to "why do you believe that?" except generated confabulation.

We need AI systems that can:

- **Know what they know** - distinguish observations from claims from verified facts from synthesized beliefs
- **Know why they know it** - trace any belief to its evidential roots
- **Revise coherently** - propagate corrections through dependent beliefs
- **Coordinate truthfully** - maintain shared understanding across agents

No existing system does all four. This repository contains our research toward solving this problem. We publish it openly because the problem is too important to solve alone.

## Our Approach

We treat agent memory as applied epistemology: stratified belief types with distinct evidence requirements, write-time coherence enforcement, and formal belief revision that preserves audit trails.

The papers here formalize this approach. We invite the research community to critique, extend, challenge, and build upon this work.

## Papers

**[Beyond Retrieval: Layered Epistemic Agent Protocol for Coherent Agent Memory](papers/whitepaper-beyond-retrieval.tex)**

The technical paper. Introduces LeAP (Layered Epistemic Agent Protocol) with stratified epistemic types, warrant functions, coherence invariants, and AGM-compliant belief revision. Presents CITE, a four-layer architecture with write-time coherence enforcement.

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
