<div align="center">

# Bitcoin Key Recovery Research

### Cryptographic Analysis of Key Space Optimization

[![Proprietary](https://img.shields.io/badge/License-Proprietary-red.svg)](LICENSE)

</div>

---

Research notebooks from key space analysis work on secp256k1. Covers bit-flip optimization, Hash160 collision analysis, Bloom filter methods, GPU-accelerated search, and RIPEMD-160 structural investigation. Organized by research area.

## Repository Structure

```
bitcoin-key-recovery-research/
├── analysis/          # Research notebooks: statistical key space analysis
├── bitflip/           # Research notebooks: bit-flip proximity and mutation strategies
├── bloom/             # Research notebooks: Bloom filter approaches for address matching
├── gpu/               # Research notebooks: GPU-accelerated key search experiments
├── hash160/           # Research notebooks: Hash160 pipeline structural analysis
└── ripemphantom/      # Research notebooks: RIPEMD-160 internal state analysis and modular exponentiation
```

## Technical Focus Areas

- **Bit-flip analysis**: Systematic evaluation of Hamming distance neighborhoods around known keys to measure fitness landscape structure
- **Hash160 pipeline**: Statistical testing of the SHA-256 to RIPEMD-160 composition for byte-position correlations and information preservation
- **Bloom filters**: Space-efficient probabilistic matching for large address sets during batch scanning
- **GPU acceleration**: CuPy and CUDA-based parallel search kernels
- **RIPEMD-160 internals**: Modular exponentiation patterns and compression function state analysis

## Requirements

- Python 3.10+
- Jupyter Notebook
- `numpy`, `coincurve` or `ecdsa`, `pycryptodome`
- Optional: `cupy`, `matplotlib`

## Author

**Andrew Dorman**
Independent Researcher -- Southlake, TX
GitHub: [ACD421](https://github.com/ACD421)
