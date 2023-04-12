
# Water Deep Potential Training Data Set 

This repo contains data used to train a Deep Neural Network Force Field for water based on SCAN functional, as described in:

*[1] Alberto Torres, Luana S. Pedroza, Marivi Fernandez-Serra, and Alexandre R. Rocha
The Journal of Physical Chemistry B 2021 125 (38), 10772-10778
DOI: 10.1021/acs.jpcb.1c04372*

*[2] Márcio S. Gomes-Filho, Alberto Torres, Alexandre Reily Rocha, and Luana S. Pedroza
The Journal of Physical Chemistry B 2023 127 (6), 1422-1428
DOI: 10.1021/acs.jpcb.2c09059*
 
## Details

1. The folder data/raw_data contains  18000 configurations [1]  in the raw format (e.g, see: https://docs.deepmodeling.com/projects/deepmd/en/master/data/data-conv.html)  
 The data folder contains six directories, named as {a, b, c, d, e, f}, meaning configurations obtained for a set of different temperatures (T = 300 and 600 K) and densities (ρ = 0.88, 1.0, and 1.2 g/cm3) (low, normal, and high density water):
	* a: 64_h2o_300K_normal_density
	* b: 64_h2o_600K_normal_density
	* c: 64_h2o_600K_low_density
	* d: 64_h2o_600K_high_density 
	* e: 64_h2o_300K_high_density 
	* f: 64_h2o_300K_low_density

2. The folder data/sub_case_deepmd_format contains  4860 configurations [2]  in  numpy format (e.g, see: https://docs.deepmodeling.com/projects/deepmd/en/master/data/data-conv.html)

It is important to mention that the Deep Neural Network Force Field was obtained from the use of the DeePMD-kit code [3]

*[3] Han Wang, Linfeng Zhang, Jiequn Han, and Weinan E. “DeePMD-kit: A deep learning package for many-body potential energy representation and molecular dynamics.” Computer Physics Communications 228 (2018): 178-184.*
