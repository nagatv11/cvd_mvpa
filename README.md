# Predicting long-term physical activity behavior in older adults with machine learning 
Cite this article if using the data: 

Thovinakere, N., Ghosh, S. S., Itturia-Medina, Y., Geddes, M.R. Social Determinants of Health and Functional Brain Connectivity Predict Long-Term Physical Activity Adherence in Older Adults After a New Cardiovascular Diagnosis. medRxiv. doi: https://doi.org/10.1101/2024.09.30.24314678

<img width="957" alt="image" src="https://github.com/user-attachments/assets/82edd3c1-ecc4-4b24-ad1a-9952506d3d4c">

# Performance results: Figure 2 and Table 3, and Sup. Figure S2

We ran three separate models using pydra-ml for which a spec file is needed where the dataset is specified. 
- behavior_model_pydra_ml.json runs demographic, cognitive and contextual features only model. Run this script using the command: pydraml -s behavior_model_pydra_ml.json
- imaging_model_pydra_ml.json runs neuroimaging features only model. Run this script using the command: pydraml -s imaging_model_pydra_ml.json
- multimodal_model_pydra_ml.json runs a multimodal model which includes all demographic, cognitive, contextual, and neuroimaging features. Run this script using the command: pydraml -s multimodal_model_pydra_ml.json

Since we ran models on a cluster, we have SLURM scripts, so the dataset should be in the same directory as the SLURM scripts.
conda create --name pydra_vfp --file requirements.txt
