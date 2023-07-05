# Machine learning guided drug discovery: application in Janus Kinase inhibitor design 

## CoGT 
[original github for CoGT](https://github.com/yingzibu/JAK_ML)
#### Set up env CoGT

```
conda remove --name CoGT --all
conda create -n CoGT python=3.9.15
conda activate CoGT
pip install jupyter 
```
chemBERTa was trained on google colab using GPU 

## MTATFP 
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



   
