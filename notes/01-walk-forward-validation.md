# Walk-forward validation beats a single train/test split

A single holdout split on time series leaks regime information: the model implicitly sees one market regime and is scored on it. Walk-forward refits on an expanding (or rolling) window and scores strictly on the next unseen block, so every score comes from a model that could actually have existed at that timestamp. The cost is compute; the benefit is that the equity curve is reconstructible in real time.
