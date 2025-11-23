# Quantum Medical Project — Unified QML + QIP (Google Colab Notebook)

This repository contains a single integrated Google Colab notebook combining Quantum Machine Learning (QML) and Quantum Image Processing (QIP) for medical diagnostics. All experiments were executed in Google Colab using Qiskit AerSimulator.

---

## Notebook Included

**Quantum_Medical_Project_QML_QIP.ipynb**

This unified notebook includes:
- Medical dataset preprocessing
- Classical ML models
- Quantum kernel computation
- QSVM (Quantum SVM)
- VQC (Variational Quantum Classifier)
- FRQI image encoding for medical images
- Quantum image reconstruction
- Sobel edge detection (classical and quantum)
- Evaluation metrics (Accuracy, F1, MSE, SSIM)

---

## Datasets Included

The following files are used directly in the Colab notebook and should be uploaded when running:

- breast_cancer.csv  
- scaler.pkl  
- pca.pkl  
- uploaded_medical.jpg  

---

## Project Structure

```
Quantum_Medical_Project.ipynb
breast_cancer.csv
scaler.pkl
pca.pkl
uploaded_medical.jpg
README.md
```

---

## 1. Quantum Machine Learning (QML)

Implemented using Qiskit (AerSimulator).

### Workflow
1. Load and preprocess dataset  
2. Standard scaling and PCA  
3. Quantum feature map and kernel  
4. QSVM and VQC implementation  
5. Compare with classical baselines  
6. Evaluate using Accuracy, F1, Precision, Recall  

### Summary of Results

| Model | Accuracy |
|-------|----------|
| SVM (RBF) | 0.95–0.97 |
| Logistic Regression | 0.96–0.97 |
| MLP | ~0.94 |
| QSVM | ~0.71 |
| VQC | ~0.63 |

---

## 2. Quantum Image Processing (QIP)

Implemented using FRQI (Flexible Representation of Quantum Images).

### Workflow
1. Convert X-ray image to grayscale  
2. Resize to 8×8  
3. Encode using FRQI  
4. Extract quantum statevector  
5. Reconstruct image  
6. Perform Sobel edge detection  
7. Compute MSE and SSIM  

### Reconstruction Quality
- MSE: ~0.18  
- SSIM: ~0.0027  

---

## How to Run in Google Colab

1. Upload the notebook to Colab  
2. Upload the dataset files when prompted  
3. Run cells sequentially  
4. Results appear directly in Colab  

---

## Conclusion

This project demonstrates the integration of Quantum Machine Learning and Quantum Image Processing for medical data analysis. Classical models still outperform quantum models on current hardware, but quantum techniques show potential for future applications. FRQI encoding successfully demonstrates how small medical images can be represented and processed at the quantum level.

The notebook provides a fully reproducible workflow suitable for academic study, research evaluation, and future extension as quantum hardware improves.

---

## Author

Mamatha Dandaboina  
Quantum Computing • Machine Learning • Medical AI Research (2025)
