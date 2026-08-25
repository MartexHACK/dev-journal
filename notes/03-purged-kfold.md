# Purged K-fold with an embargo

Standard K-fold on financial data lets a label that spans several bars overlap the boundary between train and test. Purging drops training samples whose label window intersects the test window; the embargo additionally drops a gap after the test block to kill serial correlation. Without both, cross-validated accuracy is optimistic.
