# Engrammic Research

Open research on epistemic memory for AI agents.

## The Problem

Current agent memory systems treat all stored information uniformly. A hallucination from session 1 persists with the same standing as a verified fact from session 10. Contradictions accumulate. Corrections don't propagate. The result: agents that contradict themselves, retrieve stale beliefs, and cannot explain why they believe what they believe.

## Our Thesis

Agent memory is not a retrieval problem. It is an epistemology problem.

This repository contains our research formalizing this thesis and proposing solutions. We're publishing here because we believe the problem is too important to solve alone. We invite the broader AI research community to critique, extend, and build upon this work.

## Papers

### Beyond Retrieval: Layered Epistemic Agent Protocol for Coherent Agent Memory

The technical paper. Introduces LeAP (Layered Epistemic Agent Protocol), a framework that treats agent memory as an epistemology problem with stratified epistemic types, warrant functions, coherence invariants, and AGM-compliant belief revision. Presents CITE (Context In Tiered Epistemology), a four-layer architecture implementing LeAP with write-time coherence enforcement.

[`papers/whitepaper-beyond-retrieval.tex`](papers/whitepaper-beyond-retrieval.tex)

### From Memory to Epistemics: The Architectural Case for Externalized Epistemics

The foundational argument. Presents convergent evidence from information theory, optimization theory, interpretability research, distributed systems, and neuroscience that epistemic state must be maintained external to the models doing inference.

[`papers/whitepaper-memory-to-epistemics.tex`](papers/whitepaper-memory-to-epistemics.tex)

## Contributing

We welcome contributions of all kinds:

- **Critique**: Find holes in our arguments. Point to prior work we missed. Challenge our assumptions.
- **Extensions**: Formal proofs, additional theorems, connections to other frameworks.
- **Benchmarks**: Evaluation methodologies, datasets, reproducibility improvements.
- **Implementations**: Alternative architectures satisfying LeAP axioms.

Open an issue to start a discussion, or submit a PR with proposed changes.

## Building the Papers

Requires a LaTeX distribution with standard packages. To build:

```bash
cd papers
pdflatex whitepaper-beyond-retrieval.tex
bibtex whitepaper-beyond-retrieval
pdflatex whitepaper-beyond-retrieval.tex
pdflatex whitepaper-beyond-retrieval.tex
```

## Related

- [Engrammic](https://github.com/engrammic-ai/engrammic) - Reference implementation of LeAP/CITE
- [engrammic-primitives](https://pypi.org/project/engrammic-primitives/) - Schema and type definitions

## License

Apache 2.0
