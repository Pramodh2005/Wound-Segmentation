A ConvNeXt–U-Net Architecture with Multi-Head Self-Attention for Automated Wound Segmentation

This project presents a deep learning–based automated wound segmentation system designed to accurately identify wound regions from medical images. The proposed model combines a ConvNeXt encoder, Multi-Head Self-Attention (MHSA) module, and U-Net decoder to improve feature extraction, capture global contextual information, and generate precise segmentation masks.

The system is mainly focused on diabetic foot ulcer and chronic wound segmentation, helping in automated wound assessment, treatment planning, and healing monitoring. The proposed architecture improves wound boundary detection and achieves strong segmentation performance using Dice Score and IoU metrics.

💡 Features

🩹 Automated Wound Segmentation
Accurately detects and segments wound regions from medical images.

🧠 ConvNeXt Encoder
Extracts hierarchical low-level and high-level wound features efficiently.

🌐 Multi-Head Self-Attention (MHSA)
Captures global contextual relationships and long-range dependencies for better wound localization.

🔄 U-Net Decoder with Skip Connections
Reconstructs high-resolution segmentation masks while preserving spatial information.

📈 Improved Boundary Detection
Handles irregular wound boundaries and complex textures effectively.

📊 Performance Evaluation
Evaluated using Dice Score and Intersection over Union (IoU) metrics.

🛠️ Technologies & Tools Used
Python
PyTorch
OpenCV
NumPy
Matplotlib
Scikit-learn
Kaggle Notebook / Google Colab
🧠 Model Architecture

The proposed architecture consists of:

1. ConvNeXt Encoder
Extracts hierarchical wound features
Captures edges, textures, and semantic information
2. Multi-Head Self-Attention (MHSA)
Captures global contextual information
Learns long-range dependencies between wound regions
3. U-Net Decoder
Performs upsampling and reconstruction
Uses skip connections for accurate spatial recovery
📂 Dataset

The dataset contains:

RGB wound images
Corresponding binary segmentation masks
Dataset Preprocessing
Resize images to 512×512
Image normalization
Data augmentation:
Flipping
Rotation
Brightness adjustment
Contrast enhancement
Dataset Split
Training Set → 80%
Validation Set → 10%
Testing Set → 10%
⚙️ Software Implementation
Developed using PyTorch
ConvNeXt Tiny used as encoder backbone
MHSA integrated for global feature learning
BCE + Dice Loss used for training
Trained and evaluated on wound image dataset
📚 Workflow
Input wound image is preprocessed.
ConvNeXt encoder extracts hierarchical feature maps.
MHSA module captures global contextual relationships.
U-Net decoder reconstructs segmentation masks.
Final binary wound mask is generated.
Performance evaluated using Dice and IoU metrics.
📊 Results
Model	                Dice Score (%)	IoU (%)
ConvNeXt U-Net + MHSA	88.00	          80.10
ConvNeXt U-Net	      87.88	          79.63
ConvNeXt	            87.70	          79.33

Key Observations
Improved wound boundary detection
Better segmentation accuracy
Strong performance on complex wound images
Effective handling of irregular wound regions

🚀 Future Work
Train using larger and more diverse wound datasets
Extend system for wound tissue classification
Develop mobile-based real-time wound assessment system
Integrate wound healing progression monitoring

📎 Conclusion
The proposed ConvNeXt–U-Net architecture integrated with Multi-Head Self-Attention (MHSA) provides an effective solution for automated wound segmentation. The combination of advanced feature extraction, global contextual learning, and accurate mask reconstruction significantly improves segmentation accuracy and wound boundary detection. The model demonstrates strong potential for real-world clinical wound assessment and healthcare applications.
