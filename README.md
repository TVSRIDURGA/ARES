🚀 A.R.E.S. – Advanced Radiographic Enhancement System
📌 Overview

A.R.E.S. (Advanced Radiographic Enhancement System) is an AI-powered application designed to enhance the quality of chest X-ray images using a combination of deep learning and image processing techniques.

The system improves medical image clarity by removing noise, eliminating artifacts, sharpening details, and enhancing contrast—making X-rays more suitable for analysis and diagnosis.

🎯 Problem Statement

Medical X-ray images often suffer from:

->Low contrast
->Noise and distortions
->Artifacts (unwanted bright spots or damage)

These issues reduce image clarity and can affect accurate diagnosis.

👉 This project aims to automatically enhance X-ray images to improve their visual quality using AI.

💡 Solution

The system processes uploaded X-ray images through a 6-stage enhancement pipeline that combines deep learning and image processing.

⚙️ **System Pipeline**

🔄 **6-Step Enhancement Process**

1.**Orientation**
->Image is resized and formatted for processing
->Converted to suitable input format

2.**Segmentation (Deep Learning)**
->Uses U-Net (ResNet18 encoder)
->Identifies important regions in the X-ray

3.**Denoising**
->Applies median filtering
->Removes noise from the image

4.**Artifact** **Removal**
->Uses inpainting technique
->Repairs damaged or distorted regions

5.**Sharpening (Detail Enhancement)**
->Enhances edges and structures
->Improves visual clarity

6.**Contrast Enhancement**
->Uses CLAHE (Adaptive Histogram Equalization)
->Improves brightness and contrast

🧠 Model Used
U-Net Architecture
Encoder: ResNet18
Library: segmentation_models_pytorch



📊 **Evaluation Metrics**

The system evaluates output quality using:

**PSNR (Peak Signal-to-Noise Ratio)**
  Measures noise reduction
  Higher value = better quality
  
**SSIM (Structural Similarity Index)**
  Measures structural similarity
  Higher value = better preservation
  
**Quality Grade**
  EXCELLENT / NOMINAL / ACCEPTABLE

💻 **User Interface**

Built using Streamlit, the application provides:

📤 Upload X-ray image (JPG, PNG, JPEG, WebP) 

🖼️ Display original vs enhanced image

📊 Show PSNR & SSIM metrics

📥 Download enhanced image
