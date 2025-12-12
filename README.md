🎨 Artwork Classification using Deep Learning

A CNN-based project for classifying artwork images into multiple artistic styles using Transfer Learning and Explainable AI.
This project compares three architectures: VGG16, ResNet50, EfficientNetB0 and includes a functional GUI with Grad-CAM visualization.

📂 Project Overview

This project aims to classify artwork images (painting, sketch, photography, etc.) using deep learning models.
We apply Transfer Learning, Data Augmentation, Model Evaluation, and Explainability, following the full pipeline required in the course project.
The system includes:

Dataset preprocessing

Training & tuning three CNN architectures

Visualization of metrics

Grad-CAM explainability

User-friendly GUI for prediction


📁 Repository Structure
Artwork-Classification/
│
├── data/                    
│   └── README.md
│
├── notebooks/               
│   ├── preprocessing.ipynb
│   ├── vgg16_training.ipynb
│   ├── resnet50_training.ipynb
│   └── efficientnet_training.ipynb
│
├── models/                   
│
├── gui/
│   ├── app.py                
│   └── gradcam.py            
│
├── results/                  
│   ├── accuracy.png
│   ├── confusion_matrix.png
│   └── model_comparison.png
│
├── docs/                     
│
├── requirements.txt
└── README.md

🖼️ Dataset

We use the WikiArt Dataset, which contains thousands of artwork images across many styles.
Data link: https://huggingface.co/datasets/huggan/wikiart/tree/refs%2Fconvert%2Fparquet/default/partial-train


🧠 Models Used

Three transfer-learning models were trained & compared:

Model	Parameters	Notes
VGG16	~138M	Strong baseline model
ResNet50	~25M	Deep residual learning, prevents vanishing gradients
EfficientNetB0	~5M	Lightweight and high accuracy

Each model was trained with:
Data Augmentation
Early stopping
Learning rate scheduling

📊 Model Evaluation
We evaluate all models using:
Accuracy
Precision / Recall / F1-score

Confusion Matrix
Loss Curves

Model Comparison Chart
All evaluation graphs are stored in the results/ folder.

Example:
results/
├── accuracy.png
├── confusion_matrix.png
└── model_comparison.png

🔍 Explainability – Grad-CAM

To interpret model predictions, we implemented Grad-CAM, which highlights image regions influencing the decision.

✔ Helps understand why a model classified a painting as a certain style
✔ Integrated into the GUI

Implementation in:
gui/gradcam.py

🖥️ Graphical User Interface (GUI)
A clean, simple interface built with Streamlit:

Features:
Upload any artwork image

Choose which model to use (VGG / ResNet / EfficientNet)
Display Top-3 predictions with confidence

Show Grad-CAM heatmap
Compare model performance

Run the GUI:
pip install -r requirements.txt
streamlit run gui/app.py

👥 Team Members
Role	                           Name
Data Preprocessing	
Model Training	
Evaluation & Visualization	
GUI Developer	
Documentation	


