# Prediction_of_Methionine_Oxidation_Sites
A Machine Learning Approach

The file "MetOData" is a RData containing all the data used in the paper entitled “A machine learning approach for predicting methionine oxidation sites” (BMC Bioinformatics 2017, 18:430). 

Once the file has been loaded into R, we will be able to access to a data frame formed by 975 observations (rows), one for each methionine analyzed, and 80 variables (columns). The first column provides the accession number (ACC) for the UniProtKB entry corresponding to the relevant protein. The second column gives the Protein Data Bank identifier (PDB) of the structure used for the computations. The third variable collects the methionine position within the primary structure of the protein. The fourth variable informs about whether the analyzed methionine has been detected in vivo as MetO. The remaining 76 variables are described in detail in the aforementioned paper, as well as the way they have been computed.

The file "PDBdata" is a RData containing further information regarding the list of the PDB files and protein structures analyzed in the current project.

Once the file has been loaded into R, we wil be able to access to a data frame formed by 113 observaions (rows), on for each polypeptide chain analyzed, and 4 columns:
pdb: PDB ID
chain: polypeptide chain
ACC: Uniprot accession
dif: differency in the enumeration between the sequences from Uniprot and PDB
aggregation: aggregation state of the PDB structure.

The file "Source_Code.zip", which can be downloaded from https://drive.google.com/drive/folders/0B-2Txigj940gMkRxeExWRHM2ZTA?, once it has been unzipped, contains the script ("Methionine_Oxidation_Predictive_Model.R", MOPM) that will appeal to other files (all of which are provided and they need to be present in the working directory where you are running MOPM) necessary either to extract the methionine features or to predict their oxidation status using a random forest model described in the BMC Bioinformatics paper.
