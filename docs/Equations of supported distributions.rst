.. image:: images/logo.png

-------------------------------------

Equations of supported distributions
''''''''''''''''''''''''''''''''''''

The following expressions provide the equations for the Probability Density Function (PDF), Cumulative Distribution Function (CDF), Survival Function (SF), Hazard Function (HF), and Cumulative Hazard Function (CHF) of all supported distributions. Readers should note that there are many ways to write the equations for probability distributions and careful attention should be afforded to the parametrization to ensure you understand each parameter.

Weibull Distribution
====================

:math:`\alpha = ` scale parameter :math:`\left( \alpha > 0 \right)` 

:math:`\beta = ` shape parameter :math:`\left( \beta > 0 \right)`

:math:`\text{PDF:} \hspace{11mm} f(t) = \frac{\beta t^{ \beta - 1}}{ \alpha^ \beta} e^{-(\frac{t}{\alpha })^ \beta }`

:math:`\text{CDF:} \hspace{10mm} F(t) = 1 - e^{-(\frac{t}{\alpha })^ \beta }`

:math:`\text{SF:} \hspace{14mm} R(t) = e^{-(\frac{t}{\alpha })^ \beta }`

:math:`\text{HF:} \hspace{14mm} h(t) = \frac{\beta}{\alpha} (\frac{t}{\alpha})^{\beta -1}`

:math:`\text{CHF:} \hspace{9mm} H(t) = (\frac{t}{\alpha})^{\beta}`

Exponential Distribution
========================

:math:`\lambda = ` scale parameter :math:`\left( \lambda > 0 \right)`

:math:`\text{PDF:} \hspace{11mm} f(t) = \lambda {\rm e}^{-\lambda t}`

:math:`\text{CDF:} \hspace{10mm} F(t) = 1 - {\rm e}^{-\lambda t}`

:math:`\text{SF:} \hspace{14mm} R(t) = {\rm e}^{-\lambda t}`

:math:`\text{HF:} \hspace{14mm} h(t) = \lambda`

:math:`\text{CHF:} \hspace{9mm} H(t) = \lambda t`

Normal Distribution
===================

:math:`\mu = ` location parameter :math:`\left( -\infty < \mu < \infty \right)` 

:math:`\sigma = ` scale parameter :math:`\left( \sigma > 0 \right)`

:math:`\text{PDF:} \hspace{11mm} f(t) = \frac{1}{\sigma \sqrt{2 \pi}}{\rm exp}\left[-\frac{1}{2}\left(\frac{t - \mu}{\sigma}\right)^2\right]`

:math:`\hspace{31mm} = \frac{1}{\sigma}\phi \left[ \frac{t - \mu}{\sigma} \right]`

where :math:`\phi` is the standard normal PDF with :math:`\mu = 0` and :math:`\sigma=1`

:math:`\text{CDF:} \hspace{10mm} F(t) = \frac{1}{\sigma \sqrt{2 \pi}} \int^t_{-\infty}{ {\rm exp}\left[-\frac{1}{2}\left(\frac{\theta - \mu}{\sigma}\right)^2\right]} {rm d} \theta`

:math:`\hspace{31mm} =\frac{1}{2}+\frac{1}{2}{\rm erf}\left(\frac{t - \mu}{\sigma \sqrt{2}}\right)`

:math:`\hspace{31mm} = \Phi \left( \frac{t - \mu}{\sigma} \right)`

where :math:`\Phi` is the standard normal CDF with :math:`\mu = 0` and :math:`\sigma=1`

:math:`\text{SF:} \hspace{14mm} R(t) = 1 - \Phi \left( \frac{t - \mu}{\sigma} \right)`

:math:`\hspace{31mm} = \Phi \left( \frac{\mu - t}{\sigma} \right)`

:math:`\text{HF:} \hspace{14mm} h(t) = \frac{\phi \left[\frac{t-\mu}{\sigma}\right]}{\sigma \left( \Phi \left[ \frac{\mu - t}{\sigma} \right] \right)}`

:math:`\text{CHF:} \hspace{9mm} H(t) = -{\rm ln}\left[\Phi \left(\frac{\mu - t}{\sigma}\right)\right]`

Lognormal Distribution
======================

This is a work in progress. Check back soon for more equations.

:math:`\text{PDF:} \hspace{11mm} f(t) = 1`

:math:`\text{CDF:} \hspace{10mm} F(t) = 1`

:math:`\text{SF:} \hspace{14mm} R(t) = 1`

:math:`\text{HF:} \hspace{14mm} h(t) = 1`

:math:`\text{CHF:} \hspace{9mm} H(t) = 1`

Gamma Distribution
==================

This is a work in progress. Check back soon for more equations.

:math:`\text{PDF:} \hspace{11mm} f(t) = 1`

:math:`\text{CDF:} \hspace{10mm} F(t) = 1`

:math:`\text{SF:} \hspace{14mm} R(t) = 1`

:math:`\text{HF:} \hspace{14mm} h(t) = 1`

:math:`\text{CHF:} \hspace{9mm} H(t) = 1`

Beta Distribution
=================

This is a work in progress. Check back soon for more equations.

:math:`\text{PDF:} \hspace{11mm} f(t) = 1`

:math:`\text{CDF:} \hspace{10mm} F(t) = 1`

:math:`\text{SF:} \hspace{14mm} R(t) = 1`

:math:`\text{HF:} \hspace{14mm} h(t) = 1`

:math:`\text{CHF:} \hspace{9mm} H(t) = 1`

Relationships between the 5 functions
=====================================

The PDF, CDF, SF, HF, CHF of a probability distribution are inter-related and any of these functions can be obtained from certain transformations of the others. The following transformations are useful to know, but this list is incomplete as there are many more less useful tranformations.

:math:`{\rm PDF} = frac{d}{dx} \left( {\rm CDF} \right)`
