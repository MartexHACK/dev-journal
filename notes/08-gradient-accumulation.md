# Gradient accumulation is not free

Accumulating over k microbatches emulates a k-times larger batch for the gradient, but batch-norm statistics still come from the microbatch. Models using batch-norm do not get an equivalent result; models using layer-norm do. Another reason transformers standardised on layer-norm.
