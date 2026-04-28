# A ConvNeXt–U-Net Architecture with Multi-Head Self-Attention for Automated Wound Segmentation

## 📌 Overview
This project presents a deep learning–based automated wound segmentation system designed to accurately identify wound regions from medical images. The proposed model combines a ConvNeXt encoder, Multi-Head Self-Attention (MHSA) module, and U-Net decoder to improve feature extraction, capture global contextual information, and generate precise segmentation masks.

The system is mainly focused on diabetic foot ulcer and chronic wound segmentation, helping in automated wound assessment, treatment planning, and healing monitoring.

---

# 💡 Features

- 🩹 Automated wound segmentation from medical images
- 🧠 ConvNeXt encoder for hierarchical feature extraction
- 🌐 Multi-Head Self-Attention (MHSA) for global contextual learning
- 🔄 U-Net decoder with skip connections for accurate mask reconstruction
- 📈 Improved wound boundary detection
- 📊 Performance evaluation using Dice Score and IoU metrics

---

# 🛠️ Technologies & Tools Used

- Python
- PyTorch
- OpenCV
- NumPy
- Matplotlib
- Scikit-learn
- Kaggle / Google Colab

---

# 🧠 Proposed Architecture

The proposed architecture consists of:

## 1. ConvNeXt Encoder
- Extracts low-level and high-level wound features
- Captures textures, edges, and semantic information

## 2. Multi-Head Self-Attention (MHSA)
- Captures global contextual relationships
- Learns long-range dependencies between wound regions

## 3. U-Net Decoder
- Performs upsampling and reconstruction
- Uses skip connections to preserve spatial information

---

# 📂 Dataset

The dataset contains:
- RGB wound images
- Corresponding binary segmentation masks

## Dataset Preprocessing
- Resize images to 512×512
- Image normalization
- Data augmentation:
  - Flipping
  - Rotation
  - Brightness adjustment
  - Contrast enhancement

## Dataset Split
- Training Set → 80%
- Validation Set → 10%
- Testing Set → 10%

---

# ⚙️ Software Implementation

- Developed using PyTorch
- ConvNeXt Tiny used as encoder backbone
- MHSA integrated for global contextual learning
- BCE + Dice Loss used for training
- Trained and evaluated on wound image dataset

---

# 📚 Workflow

1. Input wound image is preprocessed
2. ConvNeXt encoder extracts feature maps
3. MHSA module captures global contextual information
4. U-Net decoder reconstructs segmentation mask
5. Final binary wound mask is generated
6. Performance evaluated using Dice Score and IoU

---

# 📊 Results

| Model | Dice Score (%) | IoU (%) |
|-------|----------------|----------|
| ConvNeXt U-Net + MHSA | 88.00 | 80.10 |
| ConvNeXt U-Net | 87.88 | 79.63 |
| ConvNeXt | 87.70 | 79.33 |

## Key Observations
- Improved wound boundary detection
- Better segmentation accuracy
- Effective handling of irregular wound regions
- Strong performance on complex wound images

---

# 🚀 Future Work

- Train using larger and more diverse datasets
- Extend system for wound tissue classification
- Develop real-time mobile-based wound assessment system
- Integrate wound healing monitoring and measurement

---

# 📎 Conclusion

The proposed ConvNeXt–U-Net architecture integrated with Multi-Head Self-Attention (MHSA) provides an effective solution for automated wound segmentation. The combination of advanced feature extraction, global contextual learning, and accurate mask reconstruction significantly improves segmentation accuracy and wound boundary detection.




