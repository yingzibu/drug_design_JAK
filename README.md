# Machine learning guided drug discovery: application in Janus Kinase inhibitor design 

## CoGT only
[original github for CoGT](https://github.com/yingzibu/JAK_ML)
#### Set up env CoGT, check [environment_CoGT.yml](environment_CoGT.yml)

```
conda remove --name CoGT --all
conda create -n CoGT python=3.9.15
conda activate CoGT
pip install jupyter 
```
chemBERTa was trained using GPU, check [file](chemberta_train_cuda.ipynb)
, others trained using CPU

## MTATFP only
[original github for MTATFP](https://github.com/Yimeng-Wang/JAK-MTATFP)

#### Set up env MTATFP

```
conda create -n MTATFP python=3.9.7
conda activate MTATFP

!pip install pandas
!pip3 install torch  
!pip install rdkit  # conda install -c rdkit rdkit==2018.09.3
!pip install dgllife
!pip install dgl==1.1
!pip install molvs
!pip install matplotlib
!pip install nbconvert[webpdf]
```

check version 
```
print('conda activate MTATFP, python=3.9.7')
print('paper JAK-MTATFP for JAKi IC50 prediction')
# Python 3.9.7
!python --version 
import torch
print('torch version:', torch.__version__)             # torch version: 2.0.1
import dgl
print('dgl version: ', dgl.__version__)                # dgl version:  1.1
import dgllife
print('dglife version: ', dgllife.__version__)         # dglife version:  0.3.2
import rdkit 
print('rdkit version: ', rdkit.__version__)            # rdkit version:  2023.03.1
import molvs
print('molvs version: ', molvs.__version__)            # molvs version:  0.1.1
import matplotlib
print('matplotlib version: ', matplotlib.__version__)  # matplotlib version: 3.7.1
```


## Set up env CCM (works for CoGT + conditionalVAE + MTATFP)
For cuda version, see check [conditionalVAE.ipynb](conditionalVAE.ipynb) for conditionalVAE only or [CoGT_MTATFP_env_cuda.ipynb](CoGT_MTATFP_env_cuda.ipynb)

For local CPU verions: 

You can first create env CoGT based on the instruction above, then clone the envrionment
```
conda create --name CCM --clone CoGT
conda activate CCM
```
then install packages used for MTATFP: 
```
!pip install dgllife
!pip install dgl==1.1
!pip install molvs
```


check version 
```
!python --version 
import torch
print('torch version:', torch.__version__)              
import dgl
print('dgl version: ', dgl.__version__)                 
import dgllife
print('dglife version: ', dgllife.__version__)          
import rdkit 
print('rdkit version: ', rdkit.__version__)            
import molvs
print('molvs version: ', molvs.__version__)            
import matplotlib
print('matplotlib version: ', matplotlib.__version__)   
```
The output should be 
```
Python 3.9.15
torch version: 1.12.0
dgl version:  1.1.0
dglife version:  0.3.2
rdkit version:  2022.09.5
molvs version:  0.1.1
matplotlib version:  3.7.1
```



   
