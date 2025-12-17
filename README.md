# Mini-Project-StyleSync
# StyleSync: Multimodal AI Framework for Intelligent Fashion Recommendations

StyleSync is an AI-powered digital wardrobe system designed to automatically analyze clothing images and classify them based on **category (type)**, **color**, and **gender** using deep learning. The project supports both **Western** and **Indian (ethnic)** fashion and serves as a foundation for smart outfit recommendation and wardrobe management.

---

## 📌 Project Status

⚠️ **Important Note**

The **color identification module is currently under improvement**.  
While **clothing category** and **gender classification** perform reliably, **color prediction accuracy is not yet optimal**, especially for multi-colored garments.

This repository reflects the **current development state**, including known limitations.

---

## ✅ Implemented Features (Working)

### 1. Clothing Type Classification
- Identifies apparel categories such as:
  - Shirt, T-shirt, Trouser, Dress, Saree, Kurti, etc.
- Implemented using a **CNN backbone (ResNet-based)**.
- Achieves **high-confidence predictions** on both Western and IndoFashion datasets.

---

### 2. Gender Classification
- Classifies apparel into:
  - **Men / Women / Unisex**
- Implemented as a parallel head in a **multi-task learning architecture**.
- Performs consistently across ethnic and western clothing.

---

### 3. Multi-Task Learning Architecture
- Uses a **shared CNN backbone** with three prediction heads:
  - Category (Type)
  - Color
  - Gender
- Improves efficiency by learning shared visual features.

---

## ⚠️ Known Issue: Color Identification (Not Fully Solved)

### Current Behavior
- The model predicts **a single dominant color** per clothing item.
- Works reasonably for **single-color garments**.
- Performs poorly for:
  - Sarees
  - Printed outfits
  - Multi-colored ethnic wear

**Example Output**

<img width="816" height="910" alt="image" src="https://github.com/user-attachments/assets/3e26cc65-8517-43d5-aa6b-983b15275708" />
