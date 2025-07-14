# DiagnosAI  
> **DiagnosAI** is an open-source initiative that builds, evaluates, and shares deep-learning models for medical-image diagnostics.  
> The inaugural module, **Melanoma Detection**, implements a convolutional neural network (CNN) that flags melanoma in dermoscopic images, accelerating early-stage skin-cancer screening.

---

## Table of Contents
* [Overview](#overview)
* [Repository Structure](#repository-structure)
* [Technologies Used](#technologies-used)
* [Results](#results)
* [Getting Started](#getting-started)
* [Contributing](#contributing)
* [License](#license)

---

## Overview
Early, accurate melanoma detection can reduce the 75 % share of skin-cancer deaths it currently accounts for.  
DiagnosAI’s first release automates that screening workflow: a CNN ingests dermoscopic images, predicts malignancy, and surfaces high-risk cases to clinicians—saving manual effort and enabling faster interventions.

---

## Repository Structure
```text
DiagnosAI/
├── README.md                     # this file
└── Melanoma_Detection/
    ├── README.md                 # project-specific details
    └── Melanoma.ipynb            # full, annotated pipeline
```

---

## Technologies Used
- Python 3.9+
- TensorFlow / Keras
- NumPy & Pandas
- Augmentor (data balancing)
- Matplotlib (visualization)

---

## Results
| Dataset Variant                    | Training Accuracy | Validation Accuracy |
|------------------------------------|------------------|---------------------|
| Raw images                         | **0.9035**       | 0.2609              |
| Augmented (rotation / contrast)    | 0.4799           | 0.3043              |
| Class-rebalanced (+500 samples/cls)| **0.9566**       | **0.8151**          |

---

## Getting Started
```bash
git clone https://github.com/samuellaki/DiagnosAI.git
cd DiagnosAI/Melanoma_Detection
pip install -r requirements.txt

# launch the end-to-end notebook
jupyter notebook Melanoma.ipynb
```

## Contributing
Contributions are welcome, whether it’s improving the melanoma model, adding new disease modules, or refining documentation.

Fork the repository and create a feature branch.

Ensure code follows PEP 8 and is formatted with black.

Add or update tests where appropriate.

Open a pull request for review.

## License
DiagnosAI is released under the MIT License. 
