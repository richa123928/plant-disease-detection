# Plant Disease Detection Using CNN

PBL project for CSE0711 – Deep Learning, ITM University Gwalior.
Classifies tomato, potato and bell pepper leaf images into 15 classes using a
baseline CNN and a fine-tuned MobileNetV2, with Grad-CAM explanations.

## Dataset
PlantVillage (Kaggle): https://www.kaggle.com/datasets/emmarex/plantdisease
20,638 images, 15 classes. Not included here because of its size.

## Results (3,096 test images)
| Model | Test accuracy | Macro F1 |
|---|---|---|
| Baseline CNN | 0.8388 | 0.8137 |
| MobileNetV2 (head only) | 0.8866 | 0.8749 |
| MobileNetV2 (fine-tuned) | 0.9687 | 0.9640 |

## Files
- plant_disease_detection.ipynb: full code and outputs (Google Colab)
- plant_disease_model.keras: trained fine-tuned MobileNetV2
- class_names.json: class labels

## How to run
Upload the dataset zip to Google Drive as `plantvillage.zip`, open the notebook
in Google Colab with a T4 GPU, and run the cells from top to bottom.

## Limitation
Images are taken under controlled conditions; accuracy on field photos is not tested.
