# CoGT 
## Set up env CoGT

terminal
```
conda remove --name CoGT --all
conda create -n CoGT python=3.9.15
conda activate CoGT
pip install jupyter
jupyter notebook
```

# MTATFP 

## Set up env MTATFP

terminal
```
conda create -n MTATFP python=3.9.7
conda activate MTATFP
```

check version 
```
print('conda activate MTATFP, python=3.9.7')
print('paper JAK-MTATFP for JAKi IC50 prediction')
# Python 3.9.7
!python --version 
import torch
print('torch version:', torch.__version__) # torch version: 2.0.1
import dgl
print('dgl version: ', dgl.__version__) # dgl version:  1.1
import dgllife
print('dglife version: ', dgllife.__version__)  # dglife version:  0.3.2
import rdkit 
print('rdkit version: ', rdkit.__version__) # rdkit version:  2023.03.1
import molvs
print('molvs version: ', molvs.__version__) # molvs version:  0.1.1
import matplotlib
print('matplotlib version: ', matplotlib.__version__) # 3.7.1
```



   
