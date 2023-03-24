# MBI-MUST
MBI MUST Summer Internship Project

This is the code for my summer project at MBI, under Timothy Saunders Lab. I did stochastic modelling of morphogens, where images uploaded into the simulation determine boundaries, source and receptors, and the effective diffusion is modelled with the synthesis diffusion degradation model.


diffusion2D.ipynb models particles over 144,000 steps with set parameters. The particle density is plotted against time and the final particle image is saved as a .tiff file for processing.

receptorNoFRAP.ipynb takes in images that describe sources and receptors for the particles, where particles spawn from a source, and may bind to receptors. Particles also are unable to move within certain areas. The simulation stops when particle numbers are stable.

receptorWithFRAP.ipynb does the same as receptorNoFRAP.ipynb but with another image taken in as a region of interest. At a certain time, all particles within the ROI are removed to simulate a FRAP, and the graph will plot the time needed for the particles to return to the pre-FRAP level.
