# HyperTok

This is the companion repository for the preprint **“Unified Image Tokenization with FiLM-based Decoupling for Generation and Understanding.”**

**[Read the manuscript (PDF)](paper/HyperTok.pdf)**

Qihang Fang<sup>1</sup>, Chengcheng Tang<sup>2</sup>, and Yanchao Yang<sup>1</sup><br>
<sup>1</sup>The University of Hong Kong &nbsp;&nbsp; <sup>2</sup>Meta

## Overview

HyperTok learns one discrete visual representation for image generation and multimodal understanding. It combines:

- a shared image encoder;
- Finite Scalar Quantization (FSQ) for expressive discrete latent tokens;
- layer-wise HyperFiLM modules that produce task-specific affine parameters through cross-attention; and
- reconstruction and semantic branches trained with reconstruction and contrastive objectives.

The task-conditioned FiLM paths let the shared tokens retain low-level visual detail while remaining aligned with high-level semantics.

## Repository status

This snapshot is a **paper-only release**. It contains the manuscript and citation metadata; source code, training scripts, checkpoints, and datasets are not included. The repository does not claim that the experiments in the manuscript are currently reproducible from this snapshot alone.

## Contents

| Path | Description |
| --- | --- |
| [`paper/HyperTok.pdf`](paper/HyperTok.pdf) | Full preprint |
| [`CITATION.cff`](CITATION.cff) | Machine-readable citation metadata |
| [`MANIFEST.sha256`](MANIFEST.sha256) | SHA-256 checksum for the manuscript |

## Citation

```bibtex
@article{fang2026hypertok,
  title   = {Unified Image Tokenization with {FiLM}-based Decoupling for Generation and Understanding},
  author  = {Fang, Qihang and Tang, Chengcheng and Yang, Yanchao},
  year    = {2026},
  note    = {Preprint}
}
```

## File integrity

From the repository root, verify that the hosted manuscript matches the source artifact:

```bash
shasum -a 256 -c MANIFEST.sha256
```

The manuscript remains subject to its authors' copyright. No separate license for redistribution, modification, code, model weights, or data is granted by this repository.
