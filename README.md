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

|symbol|variable in input file|variable name from article|
|------|----------------------|--------------------------|
|t     | t | Survival time from diagnosis to nearest month + 1 |
|t'    | tprime | Maximum observied survial time from diagnosis + 1 |
|A/D   | ad | 0 - Alive, 1 - Dead |
|$`x_{0}`$ | x0 | Constant = 1.0 |
|$`x_{1}`$ | x1 | Log BUN at diagnosis |
|$`x_{2}`$ | x2 | Hemoglobin at diagnosis |
|$`x_{3}`$ | x3 | Platelets at diagnosis 0  - abnormal, 1 - normal |
|$`x_{4}`$ | x4 | Infections at diagnosis 0 - none, 1 - normal |
|$`x_{5}`$ | x5 | Age at diagnosis (complete years) |
|$`x_{6}`$ | x6 | Sex 1 - male, 2 - female |
|$`x_{7}`$ | x7 | Log WBC at diagnosis |
|$`x_{8}`$ | x8 | Fractures at diagnosis, 0 - none, 1 - present |
|$`x_{9}`$ | x9 | Log %BM at diagnosis (log % of plasma cells in bone marrow) |
|$`x_{10}`$ | x10 | % Lymphocytes in periphial blood diagnosis |
|$`x_{11}`$ | x11 | % Myeloid cells in periphial blooda t diagnosis |
|$`x_{12}`$ | x12 | Proteinuria at diagnosis |
|$`x_{13}`$  | x13 | Bence Jone protien in urine at diagnosis 1 - present, 2 - none |
|$`x_{14}`$  | x14 | Total serum  protien at diagnosis |
|$`x_{15}`$  | x15 | Serum globin (gm%) at diagnosis
|$`x_{16}`$   | x16 | Serum calcium (mgm%) at diagnosis |
