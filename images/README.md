# EntropyHub - An open source toolkit for entropic time series analysis

![EntropyHub Logo](https://github.com/MattWillFlood/EntropyHub/blob/main/Graphics/EntropyHub_profiler2.png "EntropyHub Logo")


## About

Information and uncertainty can be regarded as two sides of the same coin: 
the more uncertainty there is, the more information we gain by removing that 
uncertainty. In the context of information and probability theory, Entropy 
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
** It is important to clarify that the entropy functions herein described 
estimate entropy in the context of probability theory and information theory as
defined by Shannon, and not thermodynamic or other entropies from classical physics.**

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

Approximate Entropy - ApEn()
Sample Entropy - SampEn()
Fuzzy Entropy - FuzzEn()                               [including several fuzzy functions]
Kolmogorov Entropy - K2En()
Permutation Entropy - PermEn()                    [including weighted, amplitude-aware, edge, modified, fine-grained, and uniform-quantizaton permutation entropy variants]
Dispersion Entropy - DispEn()                        [including fine-sorted and fluctuation-based dispersion entropy variants, and reverse dispersion entropy]
corrected Conditional Entropy - CondEn()     [including Shannon entropy]
Spectral Entropy - SpecEn()                          [including band-spectral entropy]
Distribution Entropy - DistEn()
Symbolic Dynamic Entropy - SyDyEn()
Increment Entropy - IncrEn()
Cosine Similarity Entropy - CoSiEn()
Phase Entropy - PhasEn()
Slope Entropy - SlopEn()
Gridded Distribution Entropy - GridEn()       [including several Poincaré plot indices]
Bubble Entropy - BubbEn()                          [including conditional Renyí entropy]
Entropy of Entropy - EnofEn()                      [including average entropy]
Attention Entropy - AttnEn()
Cross:
Cross-Approximate Entropy - XApEn()
Cross-Sample Entropy - XSampEn()
Cross-Fuzzy Entropy - XFuzzEn()
Cross-Kolmogorov Entropy - XK2En()
Cross-Permutation Entropy - XPermEn()
corrected Cross-Conditional Entropy - XCondEn()    [including cross-Shannon entropy]
Cross-Spectral Entropy - XSpecEn()
Cross-Distribution Entropy - XDistEn()
Bidimensional:
Bidimensional Sample Entropy - SampEn2D
Bidimensional Fuzzy Entropy - FuzzEn2D
Bidimensional Distribution Entropy - DistEn2D
Multiscale:
Multiscale Entropy - MSEn()                [including coarse, modified, intrinsic-mode-function, and time-shift graining methods]
Composite Multiscale Entropy - cMSEn()   [including refined-composite multiscale entropy (rcMSEn)]
Refined Multiscale Entropy - rMSEn()   
Hierarchical Multiscale Entropy - hMSEn()   
Multiscale Cross:
Multiscale Cross-Entropy - XMSEn()                [including coarse, modified, intrinsic-mode-function, and time-shift graining methods]
Composite Multiscale Cross-Entropy - cXMSEn()   [including refined-composite multiscale cross-entropy (rcXMSEn)]
Refined Multiscale Cross-Entropy - rXMSEn()   
Hierarchical Multiscale Cross-Entropy - hXMSEn()   
License and Terms of Use
EntropyHub is licensed under the Apache License (Version 2.0) and is free to use by all on condition that the following reference be included on any outputs realized using the software:
        Matthew W. Flood and Bernd Grimm, 
        EntropyHub: An Open-Source Toolkit for Entropic Time Series Analysis, 
        2021 github.com/MattWillFlood/EntropyHub
Copyright 2021 Matthew W. Flood, EntropyHub
Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at:  http://www.apache.org/licenses/LICENSE-2.0
Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.  For Terms of Use see https://github.com/MattWillFlood/EntropyHub
A full copy of the license is available here.
Contact
If you find this package useful, please consider starring it on GitHub, MatLab File Exchange, PyPI or Julia Packages as this helps us to gauge user satisfaction.
If you have any questions about the package or identify any issues, please do not hesitate to contact us at:    entropyhubproject@gmail.com
Thank you for using EntropyHub.
Yours in research,
Matt
















A sample project that exists as an aid to the [Python Packaging User
Guide][packaging guide]'s [Tutorial on Packaging and Distributing
Projects][distribution tutorial].

This project does not aim to cover best practices for Python project
development as a whole. For example, it does not provide guidance or tool
recommendations for version control, documentation, or testing.

[The source for this project is available here][src].

Most of the configuration for a Python project is done in the `setup.py` file,
an example of which is included in this project. You should edit this file
accordingly to adapt this sample project to your needs.

----

This is the README file for the project.

The file should use UTF-8 encoding and can be written using
[reStructuredText][rst] or [markdown][md use] with the appropriate [key set][md
use]. It will be used to generate the project webpage on PyPI and will be
displayed as the project homepage on common code-hosting services, and should be
written for that purpose.

Typical contents for this file would include an overview of the project, basic
usage examples, etc. Generally, including the project changelog in here is not a
good idea, although a simple “What's New” section for the most recent version
may be appropriate.

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


We kindly ask that if you use EntropyHub in your research, to please 
include the following citation with the appropriate version number,
as well as original articles upon which functions are derived:

Matthew W. Flood, 
"EntropyHub - An open source toolkit for entropic time series analysis"
EntropyHub (v0.0), 2021, https://github.com/MattWillFlood/EntropyHub

© Copyright 2021 Matthew W. Flood, EntropyHub

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

     http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

For Terms of Use see https://github.com/MattWillFlood/EntropyHub
