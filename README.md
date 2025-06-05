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
| Mean IoU | 0.25491962 | 0.53104955| 0.5090988 |
| Dice Coefficient | 0.31672868 | 0.50593156 | 0.599607 |
| Pixel Accuracy | 0.7781333 | 0.89559335 | 0.88769466 |
| Per-Class IoU (avg.) |0.8164124 |0.900773 | 0.87267226 |
| Per-Class Dice (avg.) | 0.89892864 | 0.94779664 | 0.93200713 |

> Replace with actual results when available.
> 

---

## 🎥 Visual Outputs

📸 Includes:



- FCN prediction
  ![Screenshot from 2025-06-05 19-26-43](https://github.com/user-attachments/assets/e5032e73-5b93-4d70-907e-47b04032c932)

- UNet prediction
  ![Screenshot from 2025-06-05 19-25-33](https://github.com/user-attachments/assets/de41bf2c-802e-401d-aadb-81d29c1390a9)

- UNet++ prediction
  ![Screenshot from 2025-06-05 19-27-14](https://github.com/user-attachments/assets/628138bc-afc4-476f-858f-75732dd6658c)

  

🎥 Output videos : 
unet : 
https://drive.google.com/file/d/1BCWPqDrUAR7uq42xE2ZhZGSSJfaP_pHH/view
unet ++ :
https://drive.google.com/file/d/1rQwEJWyJwifFZe8A_IPcFmTfd0fKTe4s/view


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

🔗 [LinkedIn]([https://www.linkedin.com/in/yourprofile](https://www.linkedin.com/in/ashpak-shaikh-88a7372b0?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_contact_details%3Bv7wwAfM0Suut4XebapJt0Q%3D%3D))

Feel free to fork, star ⭐️, or open issues / pull requests! Collaboration is welcome.

---

## 📖 Related Links

- 📖 [Full Technical Blog](https://your-blog-link.com/)
- [FCN Model Checkpoints](https://drive.google.com/drive/folders/1--PCsKWNPWBxLKJh5GTQker-k-FYVDoE?usp=sharing)
- [FCN TensorBoard Data](https://drive.google.com/drive/folders/1e5xfH2OfWcU1vCDviKFd41SBKu9-B1eO?usp=sharing)
- [UNET Model Checkpoints](https://drive.google.com/drive/folders/1NImZC4otqcvOs_A9uRRB0QofDZ9SbtTi?usp=sharing)
- [UNET TensorBoard Data](https://drive.google.com/drive/folders/1HFXB6WyGJZH7JVcJtuf5b81lvcHm0vuU?usp=sharing)
- [UNET ++ Model Checkpoints](https://drive.google.com/drive/folders/17YpDYWZIkUnKXH_yHP5bAZ24eBOf6cxa?usp=sharing)
- [UNET++ TensorBoard Data](https://drive.google.com/drive/folders/1BbXT4l8ya2zE_IPoFQN1uixJRfYWzj2l?usp=sharing)
