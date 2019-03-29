# QSAR_QUEEN
MIA-QSAR modeling program
## Requirements
python >= 3
## Installing QSAR_QUEEN
QSAR_QUEEN no need to install,put the program in any directory you want.

Before your first use, open terminal and type:

$ python -m pip install --upgrade pip

$ pip install --upgrade numpy sklearn matplotlib PIL

## How to use QSAR_QUEEN
#### Draw 2D molecular structures of compounds,and each one save as a picture.The structure cannot be twisted and stretched. Font size, bond length and bond angle should be consistent. Pictures are best named with numbers. You can use any chemical drawing software you want (ChemBioDraw is recommended).Put all picture in a folder and prepare following text file:
#### 1.act.txt

It contains the bioactive value (pIC<sub>50</sub> value) of all compounds, corresponding to the name of pictures . For example, the text file will be:

>3.2

>5.4

>6.1

#### 2. test.txt (Optional)
Manually specify which compounds are used as test sets. If there is no such file, the program will randomly pick one-fifth of the compounds as a test set. For example, 12,24,27 and 32 are in the test set, the text file will be:

>12

>24

>27

>32

#### After that, copy ImageKiller.py and ImageDetective.py to this folder. Run the ImageKiller.py to align structures and generate descriptors. Run ImageDetective.py to build the model.
