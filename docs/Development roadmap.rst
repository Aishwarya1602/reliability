.. image:: images/logo.png

-------------------------------------

Development roadmap
'''''''''''''''''''

The following development roadmap is the current task list and implementation plan for the Python reliability library. I welcome the addition of new suggestions, both large and small, as well as help with writing the code if you feel that you have the ability. This roadmap is regularly changing and you may see some things remain on here for a while without progressing, while others may be prioritized at short notice. If you have a suggested feature or you find a bug, please email me (m.reid854@gmail.com) and I will endeavour to either add it rapidly (for simple tasks and bug fixes) or add it to the roadmap.

**Next task (currently in development)**

-    Add least squares as a method to obtain the initial guess for all Fitters. Currently this has been implemented in Fit_Weibull_2P_grouped but all the other Fitters use scipy which is slower but more accurate for small datasets.

**High priority (expected by the end of 2020)**

-    Limited_failure_population for Weibull_2P - Some data sets are from a population which does not all fail. Such populations are best modelled using a limited failure population model. `JMP <https://www.jmp.com/support/help/14-2/distributions-2.shtml>`_ has this distribution, but they call it "defective subpopulation". Meeker and Escobar (1998) call it "Limited Failure Population".
-    ALT_probability_plot_Weibull prints new alpha in [] when given list as input.
-    Improvement to the online documentation for how some of these methods work, including the addition of more formulas, algorithms, and better referencing.
-    Confidence intervals (both time and reliability) on the probability plots.

**Low priority (more of a wish list at this point)**

-    Logistic Distribution - This is another useful, but less common `probability distribution <https://en.wikipedia.org/wiki/Logistic_distribution>`_.
-    Cox Proportional Hazards Model - This is available in `Lifelines <https://lifelines.readthedocs.io/en/latest/Survival%20Regression.html#cox-s-proportional-hazard-model>`_.
-    Add the rank adjustment method to Nonparametric. Rank adjustment is the method used in Probability plotting (eg. to obtain the Median Ranks) and is a common and useful nonparametric estimate of the CDF, SF, and CHF.
-    3D ALT probability plots (reliability vs time vs stress). This feature is seen in `Reliasoft <http://reliawiki.com/index.php/File:ALTA6.9.png>`_.
