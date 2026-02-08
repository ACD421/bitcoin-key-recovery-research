# Bitcoin Private Key Recovery Research

Bitcoin private key recovery research: bit-flip optimization, Hash160 analysis, multi-strategy approaches.

## Overview

This repository contains research notebooks exploring various approaches to Bitcoin private key recovery through cryptographic analysis. Methods include Hamming distance optimization via bit-flipping, Hash160 byte-level analysis, GPU-accelerated key generation, and Bloom filter-based batch scanning.

## Repository Structure

```
bitflip/    - Bit-flip and Hamming distance optimization approaches
hash160/    - Hash160-level multi-strategy analysis (multi-pass SHA-256, combined ML+Bloom)
gpu/        - GPU-accelerated key generation (PyCUDA, Numba CUDA)
bloom/      - Bloom filter-based high-throughput address scanning
analysis/   - Key analysis tools, statistical distribution analysis, PDF reporting
```

## Methodology Overview

### Bit-Flip Optimization (bitflip/)
Iterative bit-flip attacks starting from known "close" private keys, measuring Hamming distance at the Hash160 level. Includes:
- Multiprocessing parallel bit-flip search (8 CPU cores)
- GPU kernel for random bit generation (Numba CUDA)
- BitflipAI: RL-inspired adaptive bit-flip strategy achieving Hash160 Hamming distance 16
- Greedy sequential bit-locking optimization (coincurve)
- Bloom filter dedup with heap-based top-N tracking

### Hash160 Analysis (hash160/)
- Multi-pass SHA-256 with modular reduction testing
- Combined PyTorch neural network + Bloom filter approaches
- scikit-learn clustering with neural network guidance

### GPU Acceleration (gpu/)
- PyCUDA-accelerated bulk key generation
- Numba CUDA kernels with Google Drive checkpointing

### Bloom Filter Scanning (bloom/)
- Probabilistic O(1) address lookup for high-throughput scanning
- CuPy GPU-accelerated Bloom filter with memory-mapped storage

### Analysis Tools (analysis/)
- Hash160 verification and derivation validation
- RIPEMD-160 output distribution statistics (byte-level mean, stdev)
- Interactive ipywidgets UI for key pattern exploration
- Compressed/uncompressed public key format analysis
- PDF report generation with reportlab

## Dependencies

- bitcoinlib, fastecdsa, coincurve, secp256k1
- PyTorch, scikit-learn
- PyCUDA, Numba, CuPy
- numpy, scipy, matplotlib
- pybloom-live, pybloomfiltermmap3

## Platform

All notebooks designed for Google Colab execution with GPU runtime.
