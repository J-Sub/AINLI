# AINLI
## Dataset
There are two datasets we used.
1. toy_CLK1.csv
2. bindingDB_CLK1.csv

### Virtual Screening
We used target (CLK1) information obtained from the EnsDTI model output (toy_CLK1.csv).
Each column in the file is formed as follows.
~~~
, com_id, pred, dpdta, dcdti, cpi, deep, mdprd, SVM, RF, MLP, zinc_id, smiles
~~~
The column we used are pred, zinc_id, smiles
Meaning of pred: The DTI prediction value of the drug for the desired target.

We hash the DTI predicted cutoff of the drug to 0.7.

### Seed Information
The CLK1 related dataset was obtained from bindingDB database (bindingDB_CLK1.csv).


## To run AINLI
```
./exe.sh 0.85
```