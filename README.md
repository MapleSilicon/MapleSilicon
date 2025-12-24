# Maple Silicon Inc.

🌐 **Website:** https://maplesilicon.co

Maple Silicon Inc. is a Canadian technology company focused on **compiler and systems infrastructure for efficient AI computation**.

Our work targets a growing gap in modern AI systems: while models increasingly exhibit **structured sparsity**, today’s software stacks largely treat computation as dense — wasting memory bandwidth, energy, and silicon capacity.

Maple Silicon’s goal is to make **sparsity a first-class, verifiable property across the ML stack**, starting at the compiler layer.

---

## What We’re Building

### SparseFlow (Primary Project)

**SparseFlow** is an MLIR-based compiler framework designed to preserve, validate, and execute **structured sparsity (N:M)** across lowering and runtime execution.

Instead of relying on backend-specific kernel tricks or opaque optimizations, SparseFlow treats sparsity as a **compiler-level contract**:

- Explicit sparsity metadata  
- Verified transformations  
- Safe fallback to dense execution when constraints are not met  

This approach improves correctness, debuggability, and long-term portability across hardware backends.

---

## Why This Matters

Modern AI hardware is constrained by:

- Memory bandwidth  
- Power limits  
- Inefficient dense execution of sparse models  

At the same time:

- Structured sparsity (e.g. 2:4) is increasingly common in production models  
- Hardware support exists but is fragile and backend-specific  
- End-to-end verification of sparsity is largely missing  

SparseFlow addresses this gap at the **compiler level**, enabling more reliable and transparent sparse execution on existing hardware.

---

## Project Status

- ✅ CPU correctness validated  
- ✅ Initial GPU functional validation completed  
- ⚠️ GPU kernels not yet performance-tuned  
- 🚧 Benchmarking and cross-vendor validation in progress  

> **Note:** SparseFlow is currently in research and development stage.  
> Performance optimization is not yet the primary goal.

---

## Open Collaboration

Maple Silicon Inc. is open to:

- Research collaboration  
- Early technical feedback  
- Pilot evaluations  
- Academic and industry discussions  

This is **foundational infrastructure** under active development, not a polished commercial product.

---

## Contact

📧 Email: info@maplesilicon.co  
🌐 Website: https://maplesilicon.co

---

## Disclaimer

SparseFlow is an experimental research project.  
APIs, behavior, and performance characteristics may change without notice.
