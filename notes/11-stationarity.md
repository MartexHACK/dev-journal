# Differencing destroys memory you may need

Making a price series stationary by taking returns throws away the level information a model might use. Fractional differentiation takes the minimum differencing order that passes an ADF test, keeping as much memory as stationarity allows.
