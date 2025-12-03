# Notes for reproducing the results of Yang and Du (2025, JAS) using CM1 model (Bryan and Fritsch, 2002).

### The CM1 version used is CM1r20.3
### The _input_sounding_ file and the _namelist.input_ used to run the CM1 simulations are archived in:
`/cm1set/`
### Before running CM1, the cold-pool dam-break CI method and the initial passive-parcel position were implemented in ./cm1_sourcecode/init3d_modified.F (you can search for “yanghp” inside the file to locate all modifications).

#### To activate these changes, replace the original file:
`cm1/src/init3d.F`
#### with the modified version:
`cm1_sourcecode/init3d_modified.F`


#### CM1 Homepage: https://www2.mmm.ucar.edu/people/bryan/cm1/
#### Bryan, G. H., and J. M. Fritsch, 2002: A benchmark simulation for moist nonhydrostatic numerical models. Mon. Wea. Rev., 130, 2917–2928, https://doi.org/10.1175/1520-0493(2002)130%253C2917:ABSFMN%253E2.0.CO;2.
