# 🧠 Semantic Segmentation with FCN, UNet & UNet++

A 5-Month Deep Learning Pipeline for Urban Scene Understanding (Cityscapes Dataset)

> Built from scratch using TensorFlow, TPU acceleration, custom training loops, and full metric tracking.
> 

---

## 📌 Project Overview

This repository contains the complete training pipelines for three semantic segmentation models:

- 🔵 FCN (Fully Convolutional Network)
- 🟢 UNet
- 🟨 UNet++

All models are trained and evaluated on the [Cityscapes Dataset](https://www.cityscapes-dataset.com/), using custom training loops, deep supervision (for UNet++), class-weighted losses, and detailed metric tracking.

> ⚙️ Built using TensorFlow 2.x + TPU (v3-8) + tf.data
> 
> 
> 🕒 Developed over 5 months (Jan 2025 – May 2025)
> 

---

## 📂 Directory Structure

```
.
├── fcn.ipynb               # Full FCN pipeline
├── unet.ipynb              # Full UNet pipeline
├── unet_plus_plus.ipynb    # Full UNet++ pipeline with deep supervision
├── README.md               # This file
└── assets/                 # Charts, sample images, output videos (optional)

```

Each notebook includes:

- Data loading & augmentation (with tf.data)
- Model architecture definition
- Custom loss functions & metrics
- TPU strategy setup
- Custom training loop
- Real-time logging & callbacks
- Output visualization

---

## 🚀 How to Run

> Recommended: Google Colab with TPU enabled
> 
1. Clone this repository:

```bash
git clone <https://github.com/ashpakshaikh26732/Unet-FCN.git>
cd Unet-FCN

```

1. Open any notebook in Jupyter/Colab:
    - `fcn.ipynb`
    - `unet.ipynb`
    - `unet_plus_plus.ipynb`
2. Upload and mount the Cityscapes dataset.
3. Run the notebook cells to:
    - Prepare data
    - Initialize model and optimizer
    - Train on TPU
    - Evaluate & visualize results

---

## 📊 Metrics Tracked

Each model logs the following during training and validation:

- Mean IoU
- Per-Class IoU
- Dice Coefficient
- Per-Class Dice Coefficient
- Pixel Accuracy

> 📉 Logged to TensorBoard and console per epoch
> 
> 
> 🎨 Visual outputs include side-by-side comparisons and video predictions
> 

---

## 📉 Sample Performance (Validation Set)

| Metric | FCN | UNet | UNet++ |
| --- | --- | --- | --- |
| Mean IoU | 0.xx | 0.xx | 0.xx |
| Dice Coefficient | 0.xx | 0.xx | 0.xx |
| Pixel Accuracy | 0.xx | 0.xx | 0.xx |
| Road IoU | 0.xx | 0.xx | 0.xx |
| Pole IoU | 0.xx | 0.xx | 0.xx |

> Replace with actual results when available.
> 

---

## 🎥 Visual Outputs

📸 Includes:

- Input image
- Ground truth label
- FCN prediction
- UNet prediction
- UNet++ prediction

🎥 Output videos or GIFs are included in the assets folder or linked below.

---

## 🧠 Highlights

- ✅ Custom training loop (not using model.fit)
- ✅ Deep supervision support for UNet++
- ✅ 5+ metrics tracked per model (train & val)
- ✅ Live logger using tqdm + IPython
- ✅ TPU-optimized with dynamic input sizes

---

## ⚠️ Known Limitations

- Reduced input resolution due to TPU memory constraints
- Cityscapes dataset must be pre-downloaded (not included)
- Training time is long for UNet++ due to deep supervision

---

## 📨 Contact & Contributions

This project was developed by:

👨‍💻 Ashpak Shaikh

📧 [ashpakshaikh26732@gmail.com](mailto:ashpakshaikh26732@gmail.com)

🔗 [LinkedIn](https://www.linkedin.com/in/yourprofile)

Feel free to fork, star ⭐️, or open issues / pull requests! Collaboration is welcome.

---

## 📖 Related Links

- 📖 [Full Technical Blog](https://your-blog-link.com/)
- 📊 [LinkedIn Project Post](https://www.linkedin.com/posts/your-post)
- 📂 [Cityscapes Dataset](https://www.cityscapes-dataset.com/)
