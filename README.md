# Multiple Myeloma data set
multiple myeloma data set with diagnostic data used for survival analysis based on visual observation of the original publication online
with a space between each dimension of each datapoint data points

# Citation
Krall JM, Uthoff VA, Harley JB. A step-up procedure for selecting variables associated with survival. Biometrics. 1975 Mar;31(1):49-57. PMID: 1164538.

# SAS Read file
```
data MultipleMyeloma;
  infile "MultipleMyeloma.prn" firstobs=2 delimiter=" ";
  input Case t tprime ad x0 x1 x2 x3 x4 x5 x6 x7 x8 x9 x10 x11 x12 x13 x14 x15 x16;
run;
```
