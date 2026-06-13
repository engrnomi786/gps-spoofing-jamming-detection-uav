# GPS Spoofing and Jamming Detection in UAVs

This repository contains the Jupyter notebook and supporting files for the research paper:

**Multi-Modal Hierarchical Fusion for Real-Time GPS Spoofing and Jamming Detection in UAVs with Uncertainty-Aware Adaptive Navigation Control**

## Overview

The project investigates GPS spoofing and jamming detection for UAV navigation using multi-modal sensor fusion. The framework combines GPS, IMU, RF, and barometric features with machine learning, deep learning, uncertainty estimation, and integrity-aware navigation control.

Main components described in the paper:

- Multi-modal feature engineering from GPS, IMU, RF, and barometric data
- Classical ML baselines such as Random Forest, XGBoost, SVM, and Logistic Regression
- Deep learning models including 1D-CNN and BiLSTM
- Uncertainty-aware inference using MC Dropout and Deep Ensembles
- VIO-based physical consistency checking
- Continuous integrity score computation for adaptive navigation control

## Repository Structure

```text
.
├── README.md
├── requirements.txt
├── LICENSE
├── CITATION.cff
├── .gitignore
├── notebooks/
│   └── gps-spoofing-jamming-detection-uav
├── src/
│   └── .gitkeep
├── data/
│   └── README.md
├── figures/
│   └── .gitkeep
├── results/
│   └── .gitkeep
└── docs/
    └── overleaf_code_availability_snippet.tex
```

## How to Use

1. Clone the repository:

```bash
git clone https://github.com/engrnomi786/gps-spoofing-jamming-detection-uav.git
cd gps-spoofing-jamming-detection-uav
```

2. Create a virtual environment:

```bash
python -m venv .venv
```

3. Activate the environment.

On Windows:

```bash
.venv\Scripts\activate
```

On macOS/Linux:

```bash
source .venv/bin/activate
```

4. Install dependencies:

```bash
pip install -r requirements.txt
```

5. Start Jupyter Notebook:

```bash
jupyter notebook
```

6. Open your notebook from the `notebooks/` folder.

## Notebook

Place your `.ipynb` file inside:

```text
notebooks/
```

Recommended notebook name:

```text
gps_spoofing_jamming_detection_uav.ipynb
```

## Data

Datasets are not included in this repository unless their licenses allow redistribution. If datasets are required, place them locally inside the `data/` folder or update the notebook paths accordingly.

Before uploading to GitHub, make sure that the notebook does not contain:

- private dataset paths
- API keys
- passwords or tokens
- personal information
- unpublished data that should not be public

## Reproducibility Notes

For best reproducibility, keep the following fixed in the notebook:

- random seed values
- train/validation/test split ratio
- package versions
- preprocessing steps
- model hyperparameters
- evaluation metrics

## Suggested Citation

If you use this code, please cite the corresponding paper:

```bibtex
@inproceedings{habib2026gpsspoofing,
  title={Multi-Modal Hierarchical Fusion for Real-Time GPS Spoofing and Jamming Detection in UAVs with Uncertainty-Aware Adaptive Navigation Control},
  author={Habib, Nauman and Ahmad, Sohail and Tariq, Muhammad},
  year={2026}
}
```

