# EntropyHub - An open source toolkit for entropic time series analysis

![EntropyHub Logo](https://github.com/MattWillFlood/EntropyHub/blob/main/Graphics/EntropyHub_profiler2.png "EntropyHub Logo")


## About

Information and uncertainty can be regarded as two sides of the same coin: 
the more uncertainty there is, the more information we gain by removing that 
uncertainty. In the context of information and probability theory, *Entropy* 
quantifies that uncertainty. 

The concept of entropy has its origins in classical physics under the second 
law of thermodynamics, a law considered to underpin our fundamental
understanding of time in physics. Attempting to analyse the analog world around
us requires that we measure time in discrete steps, but doing so compromises 
our ability to measure entropy accurately. Various measures have been derived 
to estimate entropy (uncertainty) from discrete time series, each seeking to 
best capture the uncertainty of the system under examination. This has resulted 
in many entropy statistics from approximate entropy and sample entropy, to
multiscale sample entropy and refined-composite multiscale cross-sample entropy.


As the number of statisitcal entropy measures grows, it becomes more difficult
to identify, contrast and compare the performance of each measure. To overcome
this, we have developed EntropyHub - an open-source toolkit designed to 
integrate the many established entropy methods into one package. The goal of 
EntropyHub is to provide a comprehensive set of functions with a simple and 
consistent syntax that allows the user to augment parameters at the command 
line, enabling a range from basic to advanced entropy methods to be implemented
with ease.

* It is important to clarify that the entropy functions herein described 
estimate entropy in the context of probability theory and information theory as
defined by Shannon, and not thermodynamic or other entropies from classical physics.*

## Functions

EntropyHub functions fall into 5 categories: 
Base                functions for estimating the entropy of a single univariate time series.
Cross               functions for estimating the entropy between two univariate time series.
Bidimensional       functions for estimating the entropy of a two-dimensional univariate matrix.
Multiscale          functions for estimating the multiscale entropy of a single
                    univariate time series using any of the Base entropy functions.
Multiscale Cross    functions for estimating the multiscale entropy between two 
                    univariate time series using any of the Cross-entropy functions.

### Base:

______________________________________________________|__________________
Approximate Entropy                               	  |	ApEn
Sample Entropy                                		  |	SampEn
Fuzzy Entropy                                 		  |	FuzzEn
Kolmogorov Entropy                            		  |	K2En
Permutation Entropy                           		  |	PermEn
Conditional Entropy                           		  |	CondEn
Distribution Entropy                          		  |	DistEn
Spectral Entropy                              		  |	SpecEn
Dispersion Entropy                            		  |	DispEn
Symbolic Dynamic Entropy                          	  |	SyDyEn
Increment Entropy                                 	  |	IncrEn
Cosine Similarity Entropy                         	  |	CoSiEn
Phase Entropy                                         |	PhasEn
Slope Entropy                                      	  |	SlopEn
Bubble Entropy                                		  |	BubbEn
Gridded Distribution Entropy                          |	GridEn
Entropy of Entropy                            	      |	EnofEn
Attention Entropy                                     |	AttnEn

_________________________________________________________________________
###Cross Entropies###                                       |	Function Name
______________________________________________________|__________________
Cross Sample Entropy                                  |	XSampEn
Cross Approximate Entropy                             |	XApEn
Cross Fuzzy Entropy                                   |	XFuzzEn
Cross Permutation Entropy                             |	XPermEn
Cross Conditional Entropy                             |	XCondEn
Cross Distribution Entropy                            |	XDistEn
Cross Spectral Entropy                          	  |	XSpecEn
Cross Kolmogorov Entropy                              |	XK2En
	
_________________________________________________________________________
###Bidimensional Entropies###                              |	Function Name
______________________________________________________|__________________
Bi-Dimensional Sample Entropy                         |	SampEn2D
Bi-Dimensional Fuzzy Entropy                          |	FuzzEn2D
Bi-Dimensional Distribution Entropy                   |	DistEn2D
	
_________________________________________________________________________
###Multiscale Entropy Functions#                          | Function Name
______________________________________________________|__________________ 
Multiscale Entropy                                    | MSEn
Composite/Refined-Composite Multiscale Entropy        | cMSEn
Refined Multiscale Entropy                            | rMSEn
Hierarchical Multiscale Entropy Object                | hMSEn

_________________________________________________________________________
###Multiscale Entropies###                          |	Function Name
______________________________________________________|__________________
Multiscale Sample Entropy                             |	
Multiscale Approximate Entropy                        |	
Multiscale Fuzzy Entropy                              |	
Multiscale Permutation Entropy                        |	
Multiscale Dispersion Entropy                         |	
Multiscale Cosine Similarity Entropy                  |	
Multiscale Symblic Dynamic Entropy                    |	MSobject
Multiscale Conditional Entropy                        |	     +
Multiscale Entropy of Entropy                         | MSEn / cMSEn
Multiscale Gridded Distribution Entropy               |	rMSEn / hMSEn
Multiscale Slope Entropy                              |
Multiscale Phase Entropy                              |		
Multiscale Kolmogorov Entropy                         |	
Multiscale Distribution Entropy                       |		
Multiscale Bubble Entropy                             |	
Multiscale Increment Entropy                          |	
Multiscale Attention Entropy                          |	
	
_________________________________________________________________________
###Multiscale Cross-Entropy Functions###                    | Function Name
______________________________________________________|__________________                                                     |
Multiscale Cross-Entropy                              |   XMSEn
Composite/Refined-Composite Multiscale Cross-Entropy  |   cXMSEn
Refined Multiscale Entropy                            |   rXMSEn
Hierarchical Multiscale Entropy Object                |   hXMSEn

_________________________________________________________________________
###Multiscale Cross-Entropies###                            |	Function Name
______________________________________________________|__________________
Multiscale Cross-Sample Entropy                       |	
Multiscale Cross-Approximate Entropy                  |	
Multiscale Cross-Fuzzy Entropy                        |	MSobject
Multiscale Cross-Permutation Entropy                  |	    +
Multiscale Cross-Distribution Entropy                 |	XMSEn / cXMSEn
Multiscale Cross-Kolmogorov Entropy                   | rXMSEn / hXMSEn
Multiscale Cross-Conditional Entropy                  |	



## License and Terms of Use
EntropyHub is licensed under the Apache License (Version 2.0) and is free to
use by all on condition that the following reference be included on any outputs
realized using the software:
 
        Matthew W. Flood and Bernd Grimm, 
        EntropyHub: An Open-Source Toolkit for Entropic Time Series Analysis, 
        2021 github.com/MattWillFlood/EntropyHub


**_ © Copyright 2021 Matthew W. Flood, EntropyHub

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

     http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

For Terms of Use see https://github.com/MattWillFlood/EntropyHub -**






Contact
If you find this package useful, please consider starring it on GitHub, MatLab File Exchange, PyPI or Julia Packages as this helps us to gauge user satisfaction.
If you have any questions about the package or identify any issues, please do not hesitate to contact us at:    entropyhubproject@gmail.com
Thank you for using EntropyHub.
Yours in research,
Matt


[packaging guide]: https://packaging.python.org
[distribution tutorial]: https://packaging.python.org/tutorials/packaging-projects/
[src]: https://github.com/pypa/sampleproject
[rst]: http://docutils.sourceforge.net/rst.html
[md]: https://tools.ietf.org/html/rfc7764#section-3.5 "CommonMark variant"
[md use]: https://packaging.python.org/specifications/core-metadata/#description-content-type-optional



  EntropyHub functions belong to one of five main classes/categories:
    Base Entropies             >>  e.g. Approximate Entropy (ApEn),
                                        Sample Entropy (SampEn)
    Cross Entropies            >>  e.g. Cross-Approximate Entropy (XApEn)
                                        Cross-Sample Entropy (XSampEn)
    Bidimensional Entropies    >>  e.g. Bidimensional Sample Entropy (SampEn2D)
                                        Bidimensional Fuzzy Entropy (FuzzEn2D)
    Multiscale Entropies       >>  e.g. Multiscale Sample Entropy (MSEn)
                                        Refined Multiscale Sample Entropy (rMSEn)
                                        Composite Multiscale Sample Entropy (cMSEn)
    Multiscale Cross Entropies >>  e.g. Multiscale Cross-Sample Entropy (XMSEn)
                                        Refined Multiscale Cross-Sample Entropy (rXMSEn)

_________________________________________________________________________
Base Entropies                                        |	Function Name	
______________________________________________________|__________________
Approximate Entropy                               	  |	ApEn
Sample Entropy                                		  |	SampEn
Fuzzy Entropy                                 		  |	FuzzEn
Kolmogorov Entropy                            		  |	K2En
Permutation Entropy                           		  |	PermEn
Conditional Entropy                           		  |	CondEn
Distribution Entropy                          		  |	DistEn
Spectral Entropy                              		  |	SpecEn
Dispersion Entropy                            		  |	DispEn
Symbolic Dynamic Entropy                          	  |	SyDyEn
Increment Entropy                                 	  |	IncrEn
Cosine Similarity Entropy                         	  |	CoSiEn
Phase Entropy                                         |	PhasEn
Slope Entropy                                      	  |	SlopEn
Bubble Entropy                                		  |	BubbEn
Gridded Distribution Entropy                          |	GridEn
Entropy of Entropy                            	      |	EnofEn
Attention Entropy                                     |	AttnEn

_________________________________________________________________________
Cross Entropies                                       |	Function Name
______________________________________________________|__________________
Cross Sample Entropy                                  |	XSampEn
Cross Approximate Entropy                             |	XApEn
Cross Fuzzy Entropy                                   |	XFuzzEn
Cross Permutation Entropy                             |	XPermEn
Cross Conditional Entropy                             |	XCondEn
Cross Distribution Entropy                            |	XDistEn
Cross Spectral Entropy                          	  |	XSpecEn
Cross Kolmogorov Entropy                              |	XK2En
	
_________________________________________________________________________
Bi-Dimensional Entropies                              |	Function Name
______________________________________________________|__________________
Bi-Dimensional Sample Entropy                         |	SampEn2D
Bi-Dimensional Fuzzy Entropy                          |	FuzzEn2D
Bi-Dimensional Distribution Entropy                   |	DistEn2D
	
_________________________________________________________________________
Multiscale Entropy Functions                          | Function Name
______________________________________________________|__________________ 
Multiscale Entropy Object                             | MSobject
                                                      |
Multiscale Entropy                                    | MSEn
Composite/Refined-Composite Multiscale Entropy        | cMSEn
Refined Multiscale Entropy                            | rMSEn
Hierarchical Multiscale Entropy Object                | hMSEn

_________________________________________________________________________
Multiscale Entropies	MSEn                          |	Function Name
______________________________________________________|__________________
Multiscale Sample Entropy                             |	
Multiscale Approximate Entropy                        |	
Multiscale Fuzzy Entropy                              |	
Multiscale Permutation Entropy                        |	
Multiscale Dispersion Entropy                         |	
Multiscale Cosine Similarity Entropy                  |	
Multiscale Symblic Dynamic Entropy                    |	MSobject
Multiscale Conditional Entropy                        |	     +
Multiscale Entropy of Entropy                         | MSEn / cMSEn
Multiscale Gridded Distribution Entropy               |	rMSEn / hMSEn
Multiscale Slope Entropy                              |
Multiscale Phase Entropy                              |		
Multiscale Kolmogorov Entropy                         |	
Multiscale Distribution Entropy                       |		
Multiscale Bubble Entropy                             |	
Multiscale Increment Entropy                          |	
Multiscale Attention Entropy                          |	
	
_________________________________________________________________________
Multiscale Cross-Entropy Functions                    | Function Name
______________________________________________________|__________________
Multiscale Cross-Entropy Object                       |   MSobject
                                                      |
Multiscale Cross-Entropy                              |   XMSEn
Composite/Refined-Composite Multiscale Cross-Entropy  |   cXMSEn
Refined Multiscale Entropy                            |   rXMSEn
Hierarchical Multiscale Entropy Object                |   hXMSEn

_________________________________________________________________________
Multiscale Cross-Entropies                            |	Function Name
______________________________________________________|__________________
Multiscale Cross-Sample Entropy                       |	
Multiscale Cross-Approximate Entropy                  |	
Multiscale Cross-Fuzzy Entropy                        |	MSobject
Multiscale Cross-Permutation Entropy                  |	    +
Multiscale Cross-Distribution Entropy                 |	XMSEn / cXMSEn
Multiscale Cross-Kolmogorov Entropy                   | rXMSEn / hXMSEn
Multiscale Cross-Conditional Entropy                  |	



