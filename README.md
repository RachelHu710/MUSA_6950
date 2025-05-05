# MUSA_6950 Final Project
🌿 Urban Greenery Mapping using UNet and PSPNet

This project aims to detect visible urban greenery (e.g., trees, shrubs, grass) from street-level imagery using semantic segmentation models (UNet and PSPNet). The final goal is to generate greenery density maps to support urban sustainability assessments.

📌 Project Overview
	•	Objective: Automatically segment visible greenery in street-view images using deep learning, and visualize results spatially.
	•	Models Used:
	•	UNet – accurate for fine-grained vegetation details.
	•	PSPNet – good for understanding global context in complex scenes.
	•	Application Area: Diamond Bar, CA
	•	Annotation Tool: Labelme (rectangle annotations for green_tree, shrub, grass)

 📁 Project Structure
 urban_greenery_project/
├── data/
│   ├── raw/                    # Original street images
│   ├── annotations/           # Original Labelme JSON files
│   ├── masks/                 # Converted mask images (.png)
│   └── train/
│       ├── images/            # Training images
│       └── masks/             # Training masks
│   └── test/
│       ├── images/            # Training images
│       └── masks/             # Training masks
├── models/
│   ├── unet.pth               # Trained UNet model
│   └── pspnet.pth             # Trained PSPNet model
├── notebooks/
│   ├── 01_Download_Street_Diamond.ipynb    # Download Street images in Diamond bar
│   ├── 02_Unet_train_green.ipynb    # Train UNet
│   ├── 03_PSPNet_train_green.ipynb  # Train PSPNet
│   ├── 04_eval_visualize.ipynb # Evaluate and visualize results
└── README.md
