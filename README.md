# Q-AlloSolve

## Quantum Connectivity Mapping for Blind Allosteric Site Discovery

**Q-AlloSolve** is a hybrid quantum–AI framework proposed for the **Cleveland Clinic challenge** in the **2026 Global Quantum + AI Challenge**.

**Challenge:** Unlocking Undruggable Targets: Quantum Simulation of Allosteric Signal Propagation

**Team:** QuantumForge

**Phase:** Phase 1 — Concept Proposal

## Project Objective

Q-AlloSolve investigates whether quantum graph propagation over an apo protein structure can reveal long-range residue communication patterns that improve the identification of experimentally validated allosteric regions beyond matched classical propagation methods.

The central Phase 2 research question is:

> Can quantum interference provide biologically useful connectivity information for blind allosteric site discovery that is not captured as effectively by classical diffusion over the same protein topology?

## Proposed Framework

The proposed workflow is:

~~~text
Apo Protein Structure
        ↓
Weighted Residue Interaction Graph
        ↓
Classical Graph Baselines
        ↓
AI-Guided Candidate Prioritization
        ↓
Topology-Preserving Coarse-Graining
        ↓
Quantum Graph Propagation
        ↓
Quantum Connectivity Matrix
        ↓
Quantum vs Classical Connectivity Analysis
        ↓
QUBO / QAOA Candidate Refinement
        ↓
Residue-to-Pocket Interpretation
        ↓
Top-5 Allosteric Site Predictions
        ↓
Blind Holo-Structure Validation
~~~

## Quantum Method

Protein communication is modeled using a graph-Laplacian Hamiltonian:

L = D - A

H = γL

with quantum evolution:

|ψᵢ(t)⟩ = e^(-iHt)|i⟩

Transition probabilities between residues are aggregated across controlled evolution times to construct a residue-to-residue **Quantum Connectivity Matrix**.

The Phase 2 PoC will compare quantum propagation directly against classical diffusion, random-walk, shortest-path, and graph-based baselines operating on the same protein representation.

## Benchmark Systems

| Target | Apo Input | Validation |
|---|---|---|
| KRAS G12C | 4OBE | 6OIM |
| BCR–ABL1 | 1OPL | 5MO4 |
| Cardiac Myosin | 5TBY | 6C1H |
| c-Myc | 1NKP | Exploratory |

For the strict validation targets, predictions will be generated using only the apo structure and frozen before holo-structure validation.

## Phase 2 Focus

If selected for the PoC Sprint, Q-AlloSolve will investigate:

- Blind apo-only allosteric prediction
- Explicit N × N quantum connectivity mapping
- Gate-based Hamiltonian simulation
- AI-guided search-space reduction
- Topology-preserving protein graph coarse-graining
- Quantum-vs-classical connectivity analysis
- QUBO/QAOA candidate refinement
- Quantum-noise and finite-shot robustness
- Classical-versus-quantum propagation benchmarking
- Residue-to-pocket clustering
- Interpretable 3D connectivity visualization
- AWS Braket and Classiq execution

## Hybrid Architecture

~~~text
Protein Structure
       ↓
Residue Interaction Graph
       ↓
Classical Baselines
       ↓
AI Search Reduction
       ↓
Coarse-Grained Graph
       ↓
Quantum Signal Propagation
       ↓
Quantum Connectivity Matrix
       ↓
Quantum vs Classical Analysis
       ↓
Hybrid Candidate Ranking
       ↓
Top-5 Allosteric Sites
       ↓
Blind Biological Validation
~~~

## Prior Work

QuantumForge previously developed an earlier version of **Q-AlloSolve** for the **Fujitsu Quantum Simulator Challenge 2026**.

That work explored:

- Weighted protein residue graphs
- Classical graph analysis
- AI candidate prioritization
- Graph-Laplacian quantum propagation
- QUBO/QAOA optimization
- Distributed quantum simulation using mpiQulacs

The previous work provides technical feasibility evidence and experience with KRAS, BCR–ABL1, cardiac myosin, and c-Myc.

Previous results are treated only as prior-work evidence and are not presented as validated results of the Cleveland Clinic Phase 2 methodology.

## Previous Work Report

The earlier Q-AlloSolve study developed for the **Fujitsu Quantum Simulator Challenge 2026** provides the technical foundation for the present Cleveland Clinic proposal.

The report documents prior work in weighted protein residue graphs, AI-guided candidate prioritization, graph-Laplacian quantum signal propagation, QUBO/QAOA optimization, and distributed quantum simulation using mpiQulacs.

### [Q-AlloSolve — Fujitsu Quantum Simulator Challenge 2026 Report](docs/Q-AlloSolve_Fujitsu_2026_Report.pdf)

This report is included only as evidence of prior technical work and feasibility. Its results are not presented as validated results of the proposed Cleveland Clinic Phase 2 methodology.
## Repository Structure

~~~text
Q-AlloSolve-Cleveland-2026/
│
├── README.md
│
└── docs/
    └── Q-AlloSolve_Phase1_Proposal.pdf
~~~

## Repository Status

**Current Stage:** Phase 1 — Concept Proposal Submission

If selected for Phase 2, this repository will be expanded with:

- Source code
- Protein graph construction pipeline
- Classical benchmark implementations
- Quantum circuits
- AI models
- Experiment configurations
- Noise-analysis results
- Validation outputs
- Resource estimates
- Reproducibility materials

## Team

### J K Pawan Kumar

**Team Lead — Quantum AI & Optimization**

Scientific formulation, quantum algorithm development, hybrid quantum-AI architecture, and validation strategy.

### Tarun Solanki

**Quantum/HPC Systems Lead**

Computational architecture, HPC workflows, performance profiling, infrastructure, and visualization.

## Challenge

**2026 Global Quantum + AI Challenge**

**Enterprise Partner:** Cleveland Clinic

**Problem Statement:** Unlocking Undruggable Targets: Quantum Simulation of Allosteric Signal Propagation

September 2026
