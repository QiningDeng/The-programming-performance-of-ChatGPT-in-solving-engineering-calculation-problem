# Introduction

[中文版本 (In Chinese)](README_zh.md)

Three-dimensional slope stability analysis is selected as a case study to examine the programming performance of ChatGPT in assisting in solving engineering calculation problems. Two methods of slope stability coefficient, "limit balance method" and "strength reduction method", are implemented by Python through standardized programming methods.
We propose a standardized ChatGPT programming method for 3D slope stability analysis. The limit equilibrium method is based on the three-dimensional simplified Janbu method. The geometric and mechanical parameters in each potential sliding surface area are computed traversically, and then the stability coefficient under each sliding surface is obtained. The minimum stability coefficient is obtained by comparison, and the sliding surface corresponding to it is the potential sliding surface. The strength reduction method is realized through three important parts: the calculation of finite element basic formula, the strength reduction process, the establishment of nonlinear elastic-plastic constitutive model and the Newton iteration process.

The strength reduction calculation logic theory, with the approval of the owner, refer to the MATLAB source code of "https://github.com/sysala/SSRM". 

And code testing combined with the computational theory described in the following article.

"S. Sysala, E. Hrubešová, Z. Michalec, F. Tschuchnigg: Optimization and variational principles for the shear strength reduction method. International Journal for Numerical and Analytical Methods in Geomechanics 45, 2021, pages 2388-2407."

"S. Sysala, F. Tschuchnigg, E. Hrubešová, Z. Michalec: Optimization variant of the shear strength reduction method and its usage for stability of embankments with unconfined seepage. Computers and Structures 281, 2023, 107033."

The above case uses a fixed three-dimensional slope geometry, considering the stability analysis of homogeneous soil and no groundwater. In the future, the analysis process under multi-layer soil, groundwater seepage, earthquake and other conditions will be investigated to improve the applicability.
