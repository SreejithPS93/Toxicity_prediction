Toxicity prediction using Random Forest

The dataset used consists of molecules in the form of SMILES data and their corresponding LD50 values performed on mice. SMILES is a way of encoding chemical information in the form of strings. They contain valuable information related to the structure and properties of the molecules. SMILES data can be processed using the RDKit library. 

THe SMILES string is first converted to molecule object. The morgan fingerprint of each molecule is generated. THe moragan fingerprint is 2048 bit vector. A random forest model is trained using the morgan fingerprints as features and the LD50 values as target.
