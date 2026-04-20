# Face Generation from Textual Descriptions using DCGANs

Generate realistic human faces from textual feature descriptions using **Deep Convolutional Generative Adversarial Networks (DCGANs)** and **BERT embeddings**.

---

## 📌 Overview

This project implements a **text-to-face generation system** that converts natural language descriptions of facial features into synthetic but realistic human face images.

### Key Features:
- **BERT Text Embeddings**: Encodes textual descriptions into semantic vectors
- **DCGAN Architecture**: Deep Convolutional GAN for high-quality face synthesis
- **CelebA Dataset**: Trained on diverse celebrity face images
- **Evaluation Metrics**: FIB score, Face Semantic Distance (FSD), and Face Semantic Similarity (FSS)

### Applications:
- 🎨 Art and entertainment  
- 🎮 Virtual reality and gaming  
- 🔐 Security and authentication research  
- 🏥 Medical and cosmetic visualization  
- 🔬 AI research and experimentation  

---

## 📂 Repository Structure

### File Descriptions:

| File | Purpose |
|------|---------|
| `Text_to_Face_DCGAN.ipynb` | Complete model training and generation pipeline |
| `Untitled.ipynb` | Additional experiments and testing |
| `frontend.py` | User-friendly Python interface for generating faces |
| `output*.png` | Examples of generated face images |
| `train_samples.pkl` | Pickled training sample data |

---

## 🎯 Workflow
```text
Text Description
      ↓
BERT Encoder (Embeddings)
      ↓
Latent Space Mapping
      ↓
DCGAN Generator
      ↓
Generated Face Image
```

---

## 📊 Results

Sample generated outputs are provided in the repository:

- `output1.png` - Example generation 1  
- `output5.png` - Example generation 5  
- `output10.png` - Example generation 10  
- `output11.png` - Example generation 11  
- `output15.png` - Example generation 15  
- `output20.png` - Example generation 20  
- `output50.png` - Example generation 50  

---

## 🧮 Evaluation Metrics

The model performance is evaluated using:

- **FIB Score** - Face semantic quality measurement  
- **FSD (Face Semantic Distance)** - Distance between text and generated face semantics  
- **FSS (Face Semantic Similarity)** - Similarity between text description and generated output  

---

## 🔧 Model Architecture

### DCGAN Generator:
- **Input**: BERT text embeddings (768-dimensional vectors)  
- **Process**: 5 transposed convolutional layers  
- **Output**: 120×120 RGB face images  

### DCGAN Discriminator:
- **Input**: Face images (120×120 RGB)  
- **Process**: 4 convolutional layers  
- **Output**: Real/Fake classification  

---

## 📚 Dataset

**CelebA Dataset** (Celebrity Faces Dataset)  
- 200,000+ face images  
- Pre-processed to 120×120 resolution  
- Diverse age, gender, and ethnicity representation  

---

## 🤝 Contributors

- **Pochamireddy Saivasri (POCHAMIREDDYSAIVASRI)**  
- **Nunna Srinivas Kalyan (nskalyan)**  

---

**Reference**: [CelebA Dataset](https://www.kaggle.com/datasets/jessicali9530/celeba-dataset)
