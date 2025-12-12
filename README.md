Artwork-Classification-CNN/
│
├── data/
│   └── README.md              # رابط الداتا + إزاي تتنزل
│
├── notebooks/
│   ├── preprocessing.ipynb    # تجهيز الداتا
│   ├── vgg16_training.ipynb   # أول موديل
│   ├── resnet50_training.ipynb # تاني موديل
│   └── efficientnet_training.ipynb # تالت موديل
│
├── models/
│   ├── vgg16_model.h5
│   ├── resnet50_model.h5
│   └── efficientnet_model.h5
│
├── gui/
│   ├── app.py                 # كود الواجهة Streamlit أو Tkinter
│   └── gradcam.py             # كود الجريد كام
│
├── results/
│   ├── accuracy.png
│   ├── confusion_matrix.png
│   └── model_comparison.png
│
├── docs/
│   ├── report.pdf             # التقرير النهائي
│   └── presentation.pptx      # عرض البروجكت
│
├── requirements.txt
├── README.md
└── .gitignore
