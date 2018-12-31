MuRAT - Multi-Resolution Seismic Attenuation Tomography
=======

A Matlab Package for Seismic Attenuation Tomography at multiple Earth scales using Body and Coda Waves 

MuRAT is a complete software package for measuring seismic attenuation, scattering, and absorption from passive and active data, and map 2D and 3D variations of these parameters in space.

MuRAT also comes in Python and C++ versions (under development) to provide a a fully-integrated solution for seismic attenuation imaging. 

MuRAT1.0 was first developed by Luca De Siena (Johannes Gutenberg University, Mainz, Germany) during its PhD at the INGV-Osservatorio Vesuviano, Italy, and published in 2014 while he was research assistant at the Westfälisches Wihelms Universität, Münster.

MuRAT2.0 is the the result of the activity of the Volcano Imaging group, led by De Siea during his stint as permanent Lecturer at the University of Aberdeen, UK.

The group of active users (providing questions, feedback, snippets of code) comprises De Siena's PhD students at the University of Aberdeen. It includes PhD students he co-supervises internationally. 

History
-------

* 2006-2010: The core of MuRAT (at the time named "Multi-scale reasonable attenuation tomography analysis") is based on Matlab, c++, csh and fortran codes developped at INGV-Osservatorio.
* 2010-2013: MuRAT1.0 is developed as a 3D direct-wave attenuation imaging Matlab-only code with the contribution of Christine Thomas and Richard Aster.
* 2014: MuRAT1.0 is published in De Siena et al. 2014, JVGR, with two sample datasets (Mount St. Helens and Vesuvius) [JVGR article](https://www.sciencedirect.com/science/article/abs/pii/S0377027314000961)
* 2019: MuRAT2.0 is released including 2D scattering/absorption mapping and kernel-based inversion and re-branded Multi-Resolution Seismic Attenuation Tomography. [GitHub Repository] (https://github.com/LucaDeSiena/MuRAT)


Documentation
-------------
The full documentation can be found on: ???.


Installation
------------

SYSTEM: The program works on a Macbook pro with High Sierra, Matlab R2017a.
Necessary Toolboxes: Signal Processing and Mapping (for latitute-longitude coordinates - Romania example).

Two sample datasets (Mount St. Helens and Romania) can be downloaded at https://doi.pangaea.de/10.1594/PANGAEA.893893 to test the code. A third sample input (Pollino) is provided and the related dataset may be requested to Luca De Siena.

The current version works following these steps:

1. Download the package at https://github.com/LucaDeSiena/MuRAT and unzip folder Utilities_Matlab.

2. Download the two sample datasets at https://doi.pangaea.de/10.1594/PANGAEA.893893. Unzip the MSH (Mount St. Helens) and Romania datasets and put the folders in Murat-master folder.

3. Run MuRAT5_3_6.m.


INSTRUCTIONS:

1. When asked insert the name of the input file desired (either Input_MSH.m or Input_Romania.m).

2. After the L curves are produced, pick the smoothing parameter.

3. When building your example, use one of the Input files as template. Read attentively the comments and edit only the required parameters. Start with a “pa=1” or “pa=2” analysis. “pa=3” only works with a suitable velocity model.


Citing MuRAT
--------------

If you use MuRAT for your research and publications, please consider citing it:


Disclaimer
----------

Although we have cross-checked the whole code, we cannot warranty it is exempt of bugs. The package is provided as-is, we will not be held responsible for any use you make of it, nor for the results and conclusions you may find using MuRAT.

Licence
-------

MuRAT is released under EUPL v1.1


Input file fields
-------

Analysis

Which analysis do you want to perform?
Pick delay and Qc without kernels: pa=1 
Pick delay and Qc with kernels: pa=2
Pick delay, kernel-Qc and P/S wave attenuation with the CN method: pa=3

