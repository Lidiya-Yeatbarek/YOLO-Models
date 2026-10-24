YOLO-Models: Small Object Detection in X-ray Security Scanning

Deep learning based detection of small, weak, and occluded objects in X-ray security images. This repository contains the experiments from my M.Sc. thesis at Addis Ababa Science and Technology University (AASTU):

An Ensemble Approach for Enhanced Small and Weak Object Detection in X-ray Security Scanning

Author: Lidiya Yeatbarek Bezabih Advisor: Dr. Ashenafi Yaddissa

Status: work in progress. The thesis experiments are included here. An improved version with an ensemble and updated results is currently being developed, and a paper is in preparation.

Problem

Objects in X-ray security images are often small, low-contrast, overlapping, or partly hidden by other items. Standard detectors perform well on large and clear objects but often miss these hard cases, and overall mAP can hide this weakness. This project studies how well modern YOLO detectors handle small, normal, and hidden objects, and how complementary models can be combined.

What this repository contains
Folder / file	Content
v8/	YOLOv8 training and evaluation notebooks
v9/	YOLOv9 training and evaluation notebooks
v10/	YOLOv10 training and evaluation notebooks
v11/	YOLOv11 training and evaluation notebooks
Result FSOD 60e.zip	Result files for the FSOD experiments
Datasets

The datasets are not included in this repository. Please download them from their official sources and follow their licenses.

FSOD (X-ray security dataset): [add official link]
SIXray: [add official link]

Both datasets contain small, overlapping, and partially occluded objects.

Method
Train YOLOv8, YOLOv9, YOLOv10, and YOLOv11 detectors (medium and large configurations) on the same data.
Compare Adam and SGD optimizers.
Use one shared training setup for all models, so that the comparison is fair.
Evaluate each model separately on small, normal, and hidden objects.
Combine complementary models into an ensemble based on their strengths.

Implementation: Python, PyTorch.

Training setup
Setting	Value
Framework	PyTorch (Ultralytics YOLO)
Image size	[add]
Epochs	[add]
Batch size	[add]
Optimizers	Adam, SGD
Hardware	[add GPU]
Results

Results will be added here when the improved experiments are finished.

Model	Optimizer	mAP (all)	mAP (small)	mAP (hidden)
YOLOv8				
YOLOv9				
YOLOv10				
YOLOv11				
Ensemble				
How to run
bash
# 1. Clone the repository
git clone https://github.com/Lidiya-Yeatbarek/YOLO-Models.git
cd YOLO-Models

# 2. Install requirements
pip install ultralytics torch

# 3. Download the datasets (see Datasets) and update the dataset paths in the notebooks

# 4. Open a notebook (for example v8/) and run the cells in order
Roadmap
 Compare YOLOv8 to YOLOv11 on FSOD and SIXray
 Add results tables and plots to this README
 Add the ensemble code
 Add a requirements file and clean notebook names
 Link the paper (arXiv) when it is available
Citation

A paper is in preparation. Citation details will be added here.

Contact

Lidiya Yeatbarek Bezabih Email: lidiyayeatbarek.bezabih@studenti.unipr.it LinkedIn: https://linkedin.com/in/lidiya-yeatbarek-bezabih-63a33b393 ORCID: https://orcid.org/0009-0003-8488-5714
