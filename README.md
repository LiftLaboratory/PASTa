# PASTa 1.0 
Port Access Spectral Tool alpha - a Python program to control a Biotek μQuant UV-Vis Spectrometer

Created by Patrick McArthur and Ryan Sartor at NC State University

This application can be used to control a BioTek uQuant [(mu)Quant] 96-well microplate reader.

It is written in Python and uses the pySerial library [https://github.com/pyserial/]

The Application has 3 different modes that can be selected from the UI dropdown menu:
1) Single Scan:
   This mode requires a range of wells to be specified along with a single wavelength. It will read this wavelength from all wells

2) Spectral Scan:
   Similar to single scan but a range of wavelengths is specified and each wavelength is read for each well.

3) Timecourse Scan:
   Runs a spectral scan as described above and repeats at specified intervals for a specified number of times.

All data is stored as simple .csv output files. The destination folder is specified in the UI.
