# data-quality-control-for-BREB
This program was developed to control the quality of measurement data by Bowen ratio-energy balance method based on the criteria proposed by Perez et al. 1999
%------------------Reference----------%
Perez, P., Castellvi, F., Ibanez, M., Rosell, J., 1999. Assessment of reliability of Bowen ratio method for partitioning fluxes. Agricultural and Forest Meteorology 97, 141-151
%--------------Authors----------------%
Rangjian Qiu and Zhihao Jing
Last update: Nov. 7, 2018
%-------------Cite--------------------%
If the code is useful, please cite as 
Qiu R.J., Liu C.W., Cui N.B.,Wang Z.C., Wu Y.J. , Li G., 2019. Evapotranspiration estimation using a modified Priestley-Taylor model in a rice-wheat rotation system. Agricultural Water Management, 224,105755

%--------------Input data--------------%
1.	Rn- net radiation 
2.	G-ground heat flux
3.	VP_upper- vapour pressure in the upper layer
4.	VP_lower- vapour pressure in the lower layer
5.	Bowen_ratio
6.	ET-initial Latent heat flux
7.	H-initial sensible heat flux
8.	delta_T- temperature accuracy
9.	delta_VP - vapour pressure accuracy
10.	Pa- air pressure (Kpa)
Following the steps below:
(1) Prepare the data file in excel as follows
1     2   3  4       5    6      7         8  9
Date, Time, Rn, G, VP_upper, VP-lower, Bowe_ratio, ET, H
Or you can indicate the row of each parameter in the program, but the rows of ET and H must be at the last two rows. The ‘date’ format should be number in excel file, or the matlab software cannot identify. 
(2) Indicate the total measurement data for each parameter per day (10min measurement interval, 144 data per day in this demo) in row 31 in the program.
(3) Indicate instrument temperature accuracy, vapour pressure accuracy, atmospheric pressure in rows 61-63 in the program.
(4) Make sure that the total data number of 4 days (e.g. 4*144 in the demo) could be divided by total data number
(5) Run the program
