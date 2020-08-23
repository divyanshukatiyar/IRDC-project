# Infrared Dark Clouds

Being an astrophysicist we deal with huge amounts of raw data from the sky that is needed to be converted into meaningful realizations. In this project, a section of the sky was mapped showing line emission from the infrared dark clouds among the interstellar gas. The line emission is mainly restricted to N2H+ and N2D+. We determine the deuterium fraction (N2H+/N2D+) and calculate the total column density.

## Packages used - 
aplpy, numpy, astropy, scipy, math, spectral_cube

## Steps taken -
1. Converting the raw fits file into a 3D array.
2. Slicing the data and imaging it.
3. Reading the moment maps in 2D array.
4. Loading the spectral cubes for visualization of flux vs velocity distribution (spectrum).
5. Comparing the mean spectrum for both the molecules.
6. Building contour maps for integrated intensity, column density and cloud temperature.
7. Masking some values in the moment maps to show only line emission regions.
8. Plotting and fitting column density, temperature and deuterium fraction.
9. Calculating total column density.

### Sliced cube
After reading the fits file, I sliced the data and made a scatter plot for N2D+ vs N2H+.
![$N_2D^+ vs N_2H^+$](/images/N2D+_vs_N2H+.png)

### Spectral cubes
I compared the velocity spectrum of both the molecules and increased the intensity of N2D+ to 5 times in order to match N2H+.
![spectral density](/images/vel_spec.png) ![spectral density 5 times](/images/vel_spec_factor5.png)

### Contour maps and masked moment map for N2H+
I created contour maps for integrated intensity for both the molecules, the column density and dust temperature.
![integrated intens](/images/contour_intensity_n2hp.png) ![integrated intensn2dp](/images/contour_intensity_n2dp.png)
![column density](/images/contour_coldens.png) ![temperature](/images/contour_temp.png)
![mom](/images/masked_n2hp_mom.png)

### Deuterium fraction
I have plotted the deuterium fraction against density and temperature and produced a linear fit for it.
![deuterium fraction](/images/dfrac.png)
