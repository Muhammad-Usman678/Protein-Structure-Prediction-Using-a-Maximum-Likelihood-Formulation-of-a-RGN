# Protein Structure Prediction Using a Maximum Likelihood Formulation of a Recurrent Geometric Network

## Overview
This seminar report explores the application of a **Maximum Likelihood** approach to refine protein structure prediction using the **Recurrent Geometric Network (RGN)**. The study introduces **ProteinNetX**, an enhanced version of ProteinNet, which integrates atomic displacement parameters (ADPs) and root mean square fluctuation (RMSF) data from X-ray crystallography and NMR. The main objective is to improve prediction accuracy by considering experimental uncertainties and physical realism.

## Key Sections

### 1. **Introduction**
- Understanding protein structures is crucial for therapeutic target identification.
- Deep learning models, like **AlphaFold2** and **RGN**, offer efficient alternatives to traditional physics-based methods.
- This study improves structure prediction by incorporating a **Maximum Likelihood** loss function.

### 2. **Hypothesis**
- Traditional least-squares loss functions fail to account for structural uncertainties, particularly in disordered regions.
- **Maximum Likelihood** improves model accuracy by addressing this issue and refining protein structure predictions.

### 3. **Methods and Approach**
- **ProteinNetX** integrates experimental data (B-factors, RMSF) to train a likelihood-enhanced version of **RGN**.
- The model is trained and optimized using **Amber** and **AMOEBA** forcefields to refine predictions.
- Evaluation uses geometric metrics like RMSD, GDT, and TM-score.

### 4. **Results**
- **Likelihood-RGN** outperformed traditional methods, showing better accuracy in both global and local structure predictions.
- The model demonstrated superior torsion angle predictions and better stability during physics-based optimization.

### 5. **Discussion**
- **ProteinNetX** incorporates B-factors and ADPs, enhancing prediction robustness.
- The **Maximum Likelihood** approach improves model convergence and secondary structure prediction.
- Future work will focus on refining NMR representations and enhancing protein folding models like **RGN2** and **AlphaFold2**.

## References
- Qi, G., Tollefson, M. R., Gogal, R. A., Smith, R. J. H., AlQuraishi, M., & Schnieders, M. J. (2021). "Protein structure prediction using a maximum likelihood formulation of a recurrent geometric network." bioRxiv, 2021. https://doi.org/10.1101/2021.09.03.458873
