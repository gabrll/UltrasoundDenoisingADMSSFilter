# UltrasoundDenoisingADMSSFilter
ADMSS is the Matlab© software package implementing the ‘Anisotropic Diffusion Filter with Memory based on Speckle Statistics for Ultrasound Images’ described in the recently published paper:
· G. Ramos-Llorden et al., "Anisotropic Diffusion Filter With Memory Based on Speckle Statistics for Ultrasound Images," IEEE Transactions on Image Processing, vol.24, no.1, pp.345,358, Jan. 2015 DOI: 10.1109/TIP.2014.2371244
ADMSS considerably alleviates one of the major problems of anisotropic diffusion filters [1]: the over-filtering effect due to the loss of local structures definition during the diffusion process. This is accomplished by the inclusion of a probabilistic tissue-selective memory mechanism implemented in form of a differential delay equation (DDE) for the diffusion tensor. The memory is switched off in meaningless regions but it is activated in detailed structures areas, and this distinction is performed in a Bayesian probabilistic way. As a result, the diffusion fluxes, which now follow a temporal Volterra equation, are temporally regularized and keep track of initial information only in detailed areas by giving more importance to initial diffusion fluxes than to instantaneous ones. In contrast, diffusion process continues normally in meaningless regions.
Applied to US filtering, ADMSS preserves speckle in diagnostically relevant tissues and remove it in blood regions. The probabilistic tissue characteriation is performed by means of an accurate state-of-the-art speckle characterization method, which makes use of Gamma/Normal density function mixture model [2].
If you use this code, please cite


G. Ramos-Llorden et al., "Anisotropic Diffusion Filter With Memory Based on Speckle Statistics for Ultrasound Images," IEEE Transactions on Image Processing, vol.24, no.1, pp.345,358, Jan. 2015 DOI: 10.1109/TIP.2014.2371244


The implementation of ADMSS_2D makes use of some code developed by:

Dirk-Jan Kroon (Twente University) from his Image Edge Enhancing Coherence Filter Toolbox (MATHWORKS):
derivatives.m
diffusion_scheme_2D_implicit.m
imgaussian.m
uninorm.m


Mario A. T. Figueiredo (Instituto Superior Tecnico) from his code available at: http://www.lx.it.pt/~mtf/mixturecode2.zip
mixtures4.m
multinorm.m


Gonzalo Vegas-Sanchez-Ferrero (Universidad de Valladolid):
GMMestimator.m


REFERENCES

[1] G. Ramos-Llorden et al., "Anisotropic Diffusion Filter With Memory Based on Speckle Statistics for Ultrasound Images," IEEE Transactions on Image Processing, vol.24, no.1, pp.345,358, Jan. 2015 DOI: 10.1109/TIP.2014.2371244

[2] G. Vegas-Sanchez-Ferrero et al., "Gamma mixture classifier for plaque detection in intravascular ultrasonic images,", IEEE Transactions on Ultrasonics, Ferroelectrics, and Frequency Control , vol.61, no.1, pp.44,61, January 2014 DOI: 10.1109/TUFFC.2014.6689775

![screenshot](https://github.com/gabrll/UltrasoundDenoisingADMSSFilter/assets/49204215/64dca82c-326a-48dc-8c3f-af93ef5bb4bc)



