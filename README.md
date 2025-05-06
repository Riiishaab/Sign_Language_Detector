# FastViT Hand Gesture Recognition

Real-time hand gesture recognition using state-of-the-art vision transformers.

---

## 🔑 Key Features

- **Real-time gesture recognition** through webcam integration  
- **19 different hand gestures** recognized with high accuracy  
- **Efficient model architecture** using FastViT for low-latency predictions  
- **Simple deployment** through Google Colab (no local setup required)  

---

## 🧠 Model & Architecture

This project uses the FastViT architecture, a hybrid vision transformer developed by Apple that offers an excellent balance between accuracy and computational efficiency:

- **Backbone**: `fastvit_t8.apple_in1k` pretrained model  
- **Training approach**: Transfer learning with frozen backbone  
- **Input size**: 256×256 px  
- **Classes**: 19 hand gestures  

FastViT was chosen for its efficiency advantages over other models like ConvNeXT, providing a fresh approach while maintaining high accuracy in a resource-constrained environment.

---

## 📊 Dataset

The model was trained on the Hand Gesture Recognition Image Dataset (**HaGRID**) 150k subset:

- **19 gesture classes** including common gestures like "thumbs up", "peace sign", and "stop"  
- Used the more manageable **150k version** as the full dataset is too large for training in Colab  
- Properly split between **training** and **validation** sets  

---

## 🚀 Usage

### Option 1: Run in Google Colab

1. Open the training notebook  
2. Run all cells to train the model or load pretrained weights  
3. Follow instructions for webcam integration  

### Option 2: Inference with Pretrained Model

1. Open the inference notebook  
2. Upload the pretrained model file (`sign_lang_model.pkl`)  
3. Run the webcam inference cell to start real-time detection  

---

## 📈 Results

- **97.5% accuracy** on the validation set  
- Robust performance across different lighting conditions  
- **Real-time inference capability** (>30 FPS on modern hardware)  

---

## 🔮 Future Work

- **Expanded gesture vocabulary**: Scale to cover the entire sign language alphabet and common phrases  
- **Improved deployment**: Create a standalone application for integration with video conferencing platforms  
- **Sequence modeling**: Incorporate temporal information for dynamic gesture recognition  
- **Model optimization**: Further quantization and pruning for edge device deployment  

---

## 📚 References

- [HaGRID Dataset](https://example.com/hagrid)  
- [FastViT: A Fast Hybrid Vision Transformer using Structural Reparameterization](https://example.com/fastvit)  
- [fastai Library](https://www.fast.ai/)  

---

⭐ If you find this project useful, please consider giving it a star!  
