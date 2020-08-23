# Infrared Dark Clouds

Being an astrophysicist we deal with huge amounts of raw data from the sky that is needed to be converted into meaningful realizations. In this project, a section of the sky was mapped showing line emission from the infrared dark clouds among the interstellar gas. The line emission is mainly restricted to <img src="https://render.githubusercontent.com/render/math?math=N_2H^+ and N_2D^+">. We determine the deuterium fraction ($N_2H^+$/$N_2D^+$) and calculate the total column density.

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
After reading the fits file, I sliced the data and made a scatter plot for $N_2D^+ vs N_2H^+$.
![$N_2D^+ vs N_2H^+$](N2D+_vs_N2H+.png)