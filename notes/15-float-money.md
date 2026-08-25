# Never store money in a float

0.1 plus 0.2 is not 0.3 in binary floating point. Interest and invoice arithmetic belong in integer minor units or a decimal type. Any rounding rule should be applied once, at the last step, and stated explicitly, because different jurisdictions round differently.
