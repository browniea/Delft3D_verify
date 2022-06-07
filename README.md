# Delft 3D Verify 


This code will compare experimental data to the simulated data on Delft3D.

The data calculated with Delft3D using the 18m x 4m x 2m RGDGRID shown. The turbine used is a horizontal axis and has a swept area diameter of 0.7m.  Identical to the one used to collect the experimental data. The thrust coefficient is set to 0.72 and power coefficient to 0.45.The discretization is 0.2m at the outer corners of the flume and 0.1m around the turbine placed at (6,3) as shown in the figure:

![image.png](attachment:1be26856-044a-45e1-903a-effaa255e8eb.png)



The experimental data was collected during a flume test as documented in this citation. The nondimensionalized data is documented in this paper: 
>   P. Mycek, B. Gaurier, G. Germain, G. Pinon, and E. Rivoalen, “Experimental study of the turbulence intensity effects on marine current turbines behaviour. Part I: One single turbine,” Renew. Energy, vol. 66, pp. 729–746, 2014, doi: 10.1016/j.renene.2013.12.036.  

Here is an example of re-dimensioning the experimental data. 
Nondimensionalized Centerline Data for a flume with 15% Turbulent Intensity at the inlet:

```
Velocity 15% inlet TI
   u*	y*	Downstream
0.51	0	1.2
0.595	0	2
0.788	0	3
0.862	0	4
0.911	0	5
0.913	0	6
0.927	0	7
0.953	0	8
0.965	0	9
0.954	0	10

Equations to dimensionalize: 
(u*)flow rate = raw velocity (ex:0.8 m/s)
y=0 at center of flume 
Downstream*diameter of turbine(ex:0.7)= meters downstream 
```