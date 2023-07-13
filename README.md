# Differential-Privacy-SPEML-

Differential privacy is introduced by Cynthia Dwork [1] as a set of privacy-preserving mechanisms for publicly sharing information about the dataset by descriptive characteristics rather than sharing the information about the individuals in the dataset. Differential privacy is at first achieved with simple aggregate statistics and descriptive statistics such as mean function, maximum, histograms, etc., and recently the advances with differentially private machine learning models are achieved, as well.
Differential privacy is achieved by adding noise in the process. Depending on the phase where the noise is added we differentiate:
● Input perturbation - adding noise to the input before running the algorithm
● Internal perturbation - randomizing the internals of the algorithm
● Output perturbation - add noise to the output, after running the algorithm
The goal of this exercise is to compare these approaches for achieving differential privacy, from the privacy aspect and model performance aspect and analyse the tradeoff between privacy and performance. To that end, to achieve internal perturbation, utilize a differential privacy tool that provides differentially private versions of classification and clustering models (for Python: https://github.com/IBM/differential-privacy-library, for R: https://github.com/brubinstein/diffpriv). Familiarize yourself with the differentially private mechanisms used in the chosen tool.
Secondly, apply an input perturbation and output perturbation based on the sensitivity method proposed by Dwork et al. in [1]. You may experiment with a model of your choice.
You shall analyse:
1. Input perturbation vs. internal perturbation vs. output perturbation approach on a chosen model; difference between the models’ performances, and differences to the non-private model.
2. Trade-off between privacy and model performance for every approach.
Experiments from these papers [2, 3, 4] may serve as an inspiration for the methodology of this exercise.

References:
[2] K. Chaudhuri, C. Monteleoni, and A. D. Sarwate, “Differentially Private Empirical Risk Minimization,” Journal of Machine Learning Research, vol. 12, no. Mar, pp. 1069–1109, 2011. PDF: https://arxiv.org/pdf/0912.0071.pdf
[3] K. Fukuchi, Q. K. Tran, and J. Sakuma, “Differentially Private Empirical Risk Minimization with Input Perturbation,” in Discovery Science, Cham, 2017, pp. 82–90. PDF: https://arxiv.org/pdf/1710.07425.pdf
[4] Ismat Jarin, Birhanu Eshete. DP-UTIL: Comprehensive Utility Analysis of Differential Privacy in Machine Learning. https://arxiv.org/abs/2112.12998
