# Near-to-Far-Field
Python code to compute far field radiation pattern from planar near field data. Based on description from Antenna Theory Analysis and Design Section 17.2.4 by Constantine Balanis.

# How it works
Electric field is measured across planar grid near antenna (in this case it was done in simulation as shown below)

![image](https://github.com/Jormit/Near-to-Far-Field/assets/15094591/e91653c3-2d41-494e-adc9-c4def0aa214c)

For example this is what the Ez magnitude would look across the plane

![image](https://github.com/Jormit/Near-to-Far-Field/assets/15094591/3b8f1132-fc77-4c81-a004-7f3c2b169add)

This data is exported as an .nfd file and loaded in python

![output](https://github.com/Jormit/Near-to-Far-Field/assets/15094591/c373a253-85dd-46b9-b05c-b38e9ad60a71)

A plane wave decomposition is performed by utilizing a 2D FFT

![output](https://github.com/Jormit/Near-to-Far-Field/assets/15094591/f039b1f0-e028-421d-a3b4-dcc583045fd6)

From this, the far field E field can be found over some swept angle as shown below

![output](https://github.com/Jormit/Near-to-Far-Field/assets/15094591/93877ca1-2fb0-4bc9-ad84-609bafd4e9e4)

This agrees with the simulated far field data (coordinate system is slightly different so angles aren't the same)

![image](https://github.com/Jormit/Near-to-Far-Field/assets/15094591/a641e436-0182-4aaa-81da-4515a29c7b75)

