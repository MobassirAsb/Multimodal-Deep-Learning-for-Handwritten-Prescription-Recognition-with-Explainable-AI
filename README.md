##Multimodal Deep Learning for Handwritten Prescription Recognition with Explainable AI

## 📌 Overview  
This project presents a **multimodal deep learning framework** for recognizing **Bangladeshi handwritten prescriptions** by combining **image features** with structured metadata:  
- `drug_category`  
- `dosage_form`  
- `otc_status`  

Using a **ResNet-b0 backbone** fused with metadata embeddings, our model significantly improves classification performance over unimodal CNN baselines. To enhance interpretability, **SHAP (Shapley Additive Explanations)** is integrated to explain metadata contributions.  

---

## 🔑 Key Features  
- 📂 **Custom Multimodal Dataset**: Handwritten prescription word images paired with structured metadata.  
- 🧠 **Deep Learning Models**: ResNet-b0, VGG16, and EfficientNet baselines with multimodal fusion extensions.  
- 📊 **Performance Metrics**: Accuracy, Precision, Recall, and F1-score (weighted).  
- 💡 **Explainability**: SHAP-based interpretability for metadata features.  
- ⚡ **Implementation**: PyTorch, Albumentations, NumPy, Pandas, Matplotlib.  

---

## 📊 Results  
| Model                  | Accuracy | Precision (W) | Recall (W) | F1-Score (W) |
|-------------------------|----------|---------------|------------|--------------|
| ResNet-b0 (baseline)    | 0.8654   | 0.8896        | 0.8654     | 0.8637       |
| EfficientNet-b3         | 0.8397   | 0.8654        | 0.8397     | 0.8318       |
| VGG16 (baseline)        | 0.9077   | 0.9200        | 0.9100     | 0.9150*      |
| EfficientNet-b0 (multi) | 0.9231   | 0.9331        | 0.9231     | 0.9224       |
| VGG16 (multi)           | 0.9269   | 0.9371        | 0.9269     | 0.9247       |
| **ResNet-b0 (multi)**   | **0.9449** | **0.9499** | **0.9449** | **0.9439** |

✔️ **ResNet-b0 multimodal achieved the best performance**, confirming the effectiveness of metadata fusion.  

---

---

## 🚀 Future Work  
- Expand dataset size and diversity across doctors, regions, and writing styles.  
- Incorporate **image explainability** (e.g., Grad-CAM, attention maps).  
- Explore lightweight architectures for **real-world deployment**.  
- Extend metadata to include prescription context (e.g., dosage schedule, strength).  

---


