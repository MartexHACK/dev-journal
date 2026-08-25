# Write the eval before the prompt

Without a fixed eval set, prompt iteration is a random walk that feels like progress. Twenty labelled examples covering the failure modes you care about are enough to tell a real improvement from a lucky sample, and they make regressions visible when the model version changes.
