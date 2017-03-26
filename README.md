New or modified EAGLE ULPs

Changes to make:

This ULP, while useful, makes some odd choices in the calculations. Mostly that the Imax and Resistance are calculated entirely based on the minimum tracewidth within a signal. For Imax, this may be passable, since the bottleneck could be the minimum tracewidth - but for resistance, that's just impractical! Signals can have many tracewidths throughout.

Anyway, for now, will  just change it so that it defaults to conductive ink values for r calculation. Then, move to Imax calculation based on the measurements we've done for conductive ink. From there, can investigate cleaning up the resistance calculation.


Length.ulp has a pop-up with the description, which is kinda cool. Should add that so people know what the disclaimer is.
