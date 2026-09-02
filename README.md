# Social-copying-drives-spatial-allocation-in-gregarious-herbivores
Python codes used to analyse the empirical data related to the article: Social copying drives spatial allocation in gregarious herbivores. Dataset can be found at the zenodo directory: DOI:  10.5281/zenodo.20646900 .


Most of the codes where not professionally cleaned, and as stated in the article, AI was used to generate and help in code writing, specially graphics and correct models/selections. This also means, that it might be hard to understand at some points, but most of the notebooks are very sequential, and with the data found in the zenodo directory plus the tif file in this directory it should be enough the obtain the same and similar results. The uploaded files are the following and should be run in this order:

#1 -> CLEANING.ipynb: The data popints are cleanend absed on correct GPS function, on behaviour selection (based on the article: Oro, D., Ferrer-Vilaplana, A., Bauzà, J. et al. Large herbivores and abiotic drivers jointly shape spatiotemporal grassland dynamics in a subalpine ecosystem. Sci Rep 16, 22278 (2026). https://doi.org/10.1038/s41598-026-45843-0) and saved for future use. There is a small part of clustering selection, which is not done in this notebook, but rather meant as an exploration tool. 

#2 -> CLUSTERING.ipynb: Has the clustering parameters using the density based hdbscan method. This selects regions with higher density and given a minimum number of points and distance between them determines specific cluster. 2D pictures might resemble contiguous, but there elevation has to be taken into account.

#3 -> CLUSTER-FIGURE.ipynb: plots the Figure 1 in the article, in a 2D space showing the different clusters.

#4 -> SPATIAL_DISTRIBUTION.ipynb: plots the Figure 2 in the article and makes the spatial analysis corresponding to the resting sites compared to the rest of the valley. The latest update includes a multiple sample of subsets of points in the valley and compares the medians with respect to the empirical points.

#5 -> FIGURE_3_ANALYSIS.ipynb: contains the plots and analysis related to Figure 3 in the article with the respect of the growth of newly visited sites and that of the most visited site. Different models are explored and compared between them.

#6 -> FIGURE_4_ANALYSIS.ipynb: contains the plots and analysis related to Figure 4 in the article where individual variables such as age and sociality have been studied. Plots are also included. 

#. -> utilities.py: contains the simple set_article_style() function so that all plots have the same appearance.
