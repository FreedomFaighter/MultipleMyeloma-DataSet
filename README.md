# Multiple Myeloma data set
multiple myeloma data set with diagnostic data used for survival analysis based on visual observation of the original publication online
with a space between each dimension of each datapoint data points

# Citation
Krall JM, Uthoff VA, Harley JB. A step-up procedure for selecting variables associated with survival. Biometrics. 1975 Mar;31(1):49-57. PMID: 1164538.

# SAS Read file
```
proc import datafile=‘MultipleMyeloma.csv’ out=work.multipleMyelomaSurvivalData dbms=CSV;
run;
```
