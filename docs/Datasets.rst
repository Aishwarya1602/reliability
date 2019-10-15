.. image:: images/logo.png

-------------------------------------

Datasets
''''''''

There are a few datasets that have been included with reliability that users may find useful for testing and experimenting. While this list is currently small, expect it to increase significantly over time. Within ``reliability.Datasets`` the following datasets are available:

- automotive - This dataset is relatively small and a challenging task to fit with any distribution due to its size. It also includes mostly right censored data which makes fitting more difficult.
- defective_sample - This dataset is heavily right censored with intermixed censoring (not all censored values are greater than the largest failure). It exhibits the behavior of a defective sample (aka. Limited fraction defective).

All datasets are functions which create objects and every dataset object has three values. These are:

- info - a dataframe of statistics about the dataset
- failures - a list of the failure data
- right_censored - a list of the right_censored data

If you would like more information on a dataset, you can type the name of the dataset in the help function (after importing it).

.. code:: python

    from reliability.Datasets import automotive
    print(help(automotive))

If you would like the statistics about a dataset you can access the info dataframe as shown below.

.. code:: python

    from reliability.Datasets import defective_sample
    print(defective_sample().info)

    '''
                Stat             Value
                Name  defective_sample
        Total Values             13645
            Failures      1350 (9.89%)
      Right Censored    12295 (90.11%)
    '''

The following example shows how to import a dataset and use it. Note that we must use () before accessing the failures and right_censored values.

.. code:: python

    from reliability.Datasets import automotive
    from reliability.Fitters import Fit_Weibull_2P
    Fit_Weibull_2P(failures=automotive().failures,right_censored=automotive().right_censored,show_probability_plot=False)
    
    '''
    Results from Fit_Weibull_2P (95% CI):
               Point Estimate  Standard Error      Lower CI       Upper CI
    Parameter                                                             
    Alpha       134689.767900    42803.509190  72248.433622  251096.565941
    Beta             1.153904        0.296028      0.697909       1.907835
    '''

If you have in interesting dataset, please email me (m.reid854@gmail.com) and I may include it in this database.
