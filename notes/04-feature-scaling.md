# Fit scalers inside the fold, never before it

Fitting a StandardScaler on the full dataset before splitting leaks the test set mean and variance into training. It is the single most common silent leak. The fix is a Pipeline so the scaler is refit on each training fold.
