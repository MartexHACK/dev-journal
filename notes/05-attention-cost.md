# Attention is quadratic and that is the whole design constraint

Self-attention costs O(n squared) in sequence length for both time and memory. Most long-context work is a strategy for dodging that: sliding windows, sparse patterns, low-rank approximations, or moving the memory cost off the quadratic path entirely with FlashAttention style tiling that never materialises the full matrix.
