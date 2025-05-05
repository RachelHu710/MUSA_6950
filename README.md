# 🌿 Mapping Urban Greenery Using UNet and PSPNet

This repository contains a complete pipeline for segmenting urban greenery from street-level images using semantic segmentation models (UNet and PSPNet), and evaluating the results through metrics and visualization.

---

## 📌 Overview

- **Goal:** Accurately detect visible greenery (trees, shrubs, grass) from street-view imagery.
- **Models:** UNet and PSPNet (trained from scratch).
- **Data Source:** Manually downloaded and annotated street images from Diamond Bar, California.
- **Annotation Tool:** Labelme (rectangle format).
- **Final Output:** Predicted masks + metrics + optional visualization overlays.

---

## 📁 Project Contents

### Key Files and Directories

| File / Folder                     | Description |
|----------------------------------|-------------|
| `Download_Street_Diamond.ipynb`  | (Optional) Download street-view images |
| `green_images_Diamond_bar/`      | Folder with images + `Labelme` JSON annotations |
| `test_images_Diamond_bar/`       | Test images + masks for evaluation |
| `Unet_train_green.ipynb`         | Training notebook for UNet |
| `PSPNet_train_green.ipynb`       | Training notebook for PSPNet |
| `eval_visualize.ipynb`           | Evaluation and visualization notebook |
| `unet_greenery_segmentation.pth` | Trained UNet model weights |
| `pspnet_greenery.pth`            | Trained PSPNet model weights |
| `Final_Project_Proposal_Nature`  | Project proposal draft |
| `MUSA_6950.pdf`                  | Final project presentation |
| `Final_pytorch_mask_r_cnn.ipynb`| [Optional] earlier experiment with Mask R-CNN |
