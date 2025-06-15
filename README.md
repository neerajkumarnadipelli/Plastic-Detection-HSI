# Plastic Detection in Hyperspectral Images

## 📘 Overview

Hyperspectral imaging (HSI) is a powerful remote sensing technique to detect plastic waste due to the unique spectral signatures of materials.  
However, the absence of pixel-level ground truth for plastic materials makes real-world validation difficult.

To overcome this, we:
- Generated synthetic hyperspectral data using known plastic spectral signatures.
- Benchmarked spectral unmixing algorithms like FCLS, NNLS, KHype, NMF, ElasticNet, LASSO, UCLS, Pseudo-Inverse.
- Applied top-performing models to real AVIRIS hyperspectral imagery from four Indian coastal regions.

---

## 📂 Repository Structure

| File | Description |
|------|-------------|
| `Synthetic Data Generation & Evaluation.ipynb` | Generates synthetic HSI using a spectral library and evaluates 8 unmixing algorithms. Outputs include abundance maps and performance metrics like RMSE, MAE, and SAD. |
| `Plastic_Detection.ipynb` | Applies selected models (FCLS, NNLS) to real AVIRIS data of Veraval, Kochi, Mangalore, and Kolkata. Visualizes abundance maps of plastics. |

---

## 🛠️ Requirements

```bash
pip install numpy pandas scipy matplotlib scikit-learn
