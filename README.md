<div align="center">

# Bitcoin Key Recovery Research

### Cryptographic Analysis of Key Space Optimization

**Bit-flip optimization | Hash160 analysis | Multi-strategy approaches**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

</div>

## Overview

Academic research into the mathematical properties of Bitcoin's key derivation and address generation. This work explores optimization strategies for key space search, including bit-flip heuristics, Hash160 collision analysis, and multi-strategy combinatorial approaches.

## Research Focus

- **Bit-flip optimization**: Measuring how key proximity in bit-space correlates with address proximity
- **Hash160 analysis**: Statistical properties of RIPEMD-160(SHA-256(pubkey)) mapping
- **Multi-strategy search**: Combining analytical and heuristic approaches

## Disclaimer

This is academic cryptographic research. The mathematical hardness of ECDLP on secp256k1 makes brute-force key recovery computationally infeasible. This work studies the *structure* of the problem, not practical attacks.

## Related

- [secp256k1-geometric-analysis](https://github.com/ACD421/secp256k1-geometric-analysis) -- Geometric properties of the curve
- [bitcoin-puzzle-solvers](https://github.com/ACD421/bitcoin-puzzle-solvers) -- Challenge puzzle approaches
- [QRTB](https://github.com/ACD421/qrtb) -- Post-quantum alternative

## Author

**Andrew C. Dorman** -- [Hollow Point Labs](https://github.com/ACD421)

## License

MIT
