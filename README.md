# Data and Code for paper - MedSim

### Folder Specification
- ```data/```
    - **procesing.py** data preprocessing file.
    - **ndc2atc_level4.csv**: a NDC-RXCUI-ATC4 mapping file, and we only need the RXCUI to ATC4 mapping. 
    - **drug-atc.csv**: this is a CID-ATC file, which gives the mapping from CID code to detailed ATC code.
    - **ndc2rxnorm_mapping.csv**: rxnorm to RXCUI mapping file.
    - **drug-DDI.csv**: this a large file, containing the drug DDI information, coded by CID. The file could be downloaded from https://drive.google.com/file/d/1mnPc0O0ztz0fkv3HF-dpmBb8PLWsEoDz/view?usp=sharing
    - **atc2rxnorm.pkl**: drug ID dict.
    - **ddi_A_final.pkl**: ddi adjacency matrix
    - **ehr_adj_final.pkl****: used in GAMENet baseline.
    - **records_final.pkl**: The final diagnosis-procedure-medication EHR records of each patient.
    - **voc_final.pkl**: diag/prod/med index to code dictionary
- ```src/```
    - **MedSim.py**: our model
    - baselines:
        - **GAMENet.py**
        - **DMNC.py**
        - **Leap.py**
        - **Retain.py**
        - **LR.py**
