# Why warmup works

At initialisation, Adam second-moment estimates are based on almost no data, so early updates have very high variance. Warmup keeps the step size small until those estimates stabilise. This is also why an optimiser with bias correction plus warmup is more robust than either alone.
