# Pre-norm vs post-norm transformers

Post-norm (original) puts LayerNorm after the residual add and needs learning-rate warmup to train deep stacks stably. Pre-norm puts it inside the residual branch, giving a clean identity path to the output, which trains deep models without warmup at a small cost in final quality. Nearly all modern large models are pre-norm.
