# X-Ray analysis using deep learning

This repository focuses on a medical image classification project aimed at diagnosing conditions based on chest X-rays. Using advanced deep learning techniques, we implemented a DenseNet121 model, along with federated learning approaches, to train and evaluate performance on a large-scale medical dataset. 

**For detailed insights and results, refer to the project report included in this repository.**

Dataset Used:
The dataset used in this research was sourced from a well-known repository of medical imaging studies (CheXpert). Due to its large size and complexity, it provides a robust platform for evaluating the capabilities of modern deep learning techniques in healthcare.

# Required Environment

- Python 
- NumPy
- PyTorch 
- Matplotlib
- SkLearn
- GPU environment

# Results

The performance of our model is evaluated by comparing the AUC scores obtained in our experiments against those reported in the original paper. Below is a summary of the results: <br><br>


<p align="center">
    <img src="https://github.com/user-attachments/assets/600b5d09-a989-4d93-91a4-65dbaaa652d9" alt="ROC Curve 1" width="180">
    <img src="https://github.com/user-attachments/assets/5166ee17-b472-4056-b982-6327a75870c6" alt="ROC Curve 2" width="180">
    <img src="https://github.com/user-attachments/assets/e3f611a1-277a-49ad-970f-743c86a75ec5" alt="ROC Curve 3" width="185">
    <img src="https://github.com/user-attachments/assets/e3f611a1-277a-49ad-970f-743c86a75ec5" alt="ROC Curve 4" width="185">
    <img src="https://github.com/user-attachments/assets/6b16c861-4168-46bd-bbd2-dbd816d43202" alt="ROC Curve 4" width="190">
</p>  

<br><br>

Condition	AUC| (Our Model)|	AUC (Original Paper)| Difference 
--- | --- | --- | --- 
Consolidation|	0.75| 0.90| -0.15
Edema| 0.90|	0.92|  -0.02
Pleural Effusion| 	0.93|	0.97|  -0.04
Cardiomegaly| 	0.93|	0.90|  +0.03
Atelectasis| 	0.82|	0.85|  -0.03
Average AUC|  0.86|  0.91|  -0.05  

<br><br>

Our model performs closely to the baseline results reported in the original paper, with only some deviation. This shows that we have room for improvement, perhaps deploying certain strategies mention in the report may help. For detailed analysis and visualizations (e.g., ROC curves), please refer to the accompanying report in the repository.

# References 

[1] CheXpert: A Large Chest Radiograph Dataset with Uncertainty Labels and Expert Comparison, Irvin et al., 20

[2] Communication-Efficient Learning of Deep Networks from Decentralized Data, McMahan et al., 2017
