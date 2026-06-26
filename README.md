# flock-bench

Benchmarks of the [Flock](https://github.com/succinctlabs/flock) zero-knowledge prover on an **Apple M5 Max**, compared against Binius64, Hashcaster, and Plonky3.

**[View the results →](https://soispoke.github.io/flock-bench/)**

## What's measured

Hash-compression proving throughput (keccak-f[1600], SHA-256, BLAKE3) plus prove/verify time, proof size, and peak memory. Cross-prover rows are at a matched 12 threads; Flock is shown in fast, secure (~120-bit), and slim (rate 1/4) configurations.

## Notes

- Numbers are best-of-3 after warm-up on a quiet machine; throughput = hashes ÷ end-to-end prove time (witness/trace gen included).
- Security targets differ slightly between systems (~96–101 bits, Flock-secure ~120) and are labeled inline.
- Rows prove **N independent** compressions, not a hash chain.

Single-page site — `index.html` is the report; open it directly or via the link above.
