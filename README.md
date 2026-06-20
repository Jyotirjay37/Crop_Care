# 🌾 Crop Care+

> **Smart Agriculture Made Simple** | AI-Powered Crop Health Monitoring & Disease Detection

---

## 🎯 Overview

**Crop Care+** is an intelligent agricultural solution designed to help farmers and agricultural professionals monitor crop health, detect diseases early, and make data-driven decisions to maximize yield and sustainability.

Using cutting-edge machine learning and computer vision, Crop Care+ analyzes crop images and provides:
- 🔍 **Real-time disease detection**
- 📊 **Crop health analysis**
- 💡 **Smart recommendations**
- 📈 **Performance insights**

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 🤖 **AI-Powered Disease Detection** | Identify crop diseases from images with high accuracy |
| 📸 **Image Analysis** | Upload crop/leaf images for instant analysis |
| 🎯 **Crop Classification** | Recognize and classify different crop types |
| ⚠️ **Early Warning System** | Get alerts before diseases spread |
| 📊 **Health Score** | Real-time crop health metrics and statistics |
| 💾 **Data History** | Track crop health over time |
| 🌍 **Multi-Crop Support** | Works with various crops (Rice, Wheat, Corn, etc.) |
| 📱 **User-Friendly Interface** | Easy-to-use dashboard and visualizations |

---

## 🛠️ Installation

### Prerequisites
- 🐍 Python 3.8 or higher
- 📦 pip (Python Package Manager)
- 🎓 Jupyter Notebook (optional, for running notebooks)

### Step 1: Clone the Repository

```bash
git clone https://github.com/Jyotirjay37/Crop_Care.git
cd Crop_Care
```

### Step 2: Create Virtual Environment (Recommended)

```bash
# Create virtual environment
python -m venv venv

# Activate virtual environment
# On Windows:
venv\Scripts\activate

# On macOS/Linux:
source venv/bin/activate
```

### Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 4: Verify Installation

```bash
python -c "import tensorflow; import cv2; print('✅ All dependencies installed successfully!')"
```

---

## 🚀 Quick Start

### Option 1: Using Jupyter Notebook (Recommended for Beginners)

```bash
jupyter notebook
# Navigate to the notebook file and run cells sequentially
```

### Option 2: Command Line Interface

```bash
python main.py --image path/to/crop_image.jpg
```

### Option 3: Interactive Web Interface

```bash
streamlit run app.py
```

---

## 📖 Usage Guide

### Basic Workflow

```
┌─────────────────────────────────────────┐
│     Upload Crop/Leaf Image              │
└────────────────┬────────────────────────┘
                 │
                 ▼
┌─────────────────────────────────────────┐
│   Image Processing & Preprocessing      │
└────────────────┬────────────────────────┘
                 │
                 ▼
┌─────────────────────────────────────────┐
│   AI Model Inference                    │
│   (Disease Detection & Classification)  │
└────────────────┬────────────────────────┘
                 │
                 ▼
┌─────────────────────────────────────────┐
│   Generate Results & Recommendations    │
│   - Disease Type                        │
│   - Confidence Score                    │
│   - Treatment Suggestions               │
└─────────────────────────────────────────┘
```

---

## 🎓 How to Use

### 1️⃣ **Prepare Your Image**

- 📸 Take a clear photo of the affected crop/leaf
- 🌞 Ensure good lighting
- 🎯 Keep the crop in focus (at least 70% of the image)
- 📐 Supported formats: `.jpg`, `.jpeg`, `.png`

### 2️⃣ **Run Analysis**

**Example 1: Python Script**
```python
from crop_care import CropAnalyzer

# Initialize analyzer
analyzer = CropAnalyzer(model_path='models/crop_detection_model.h5')

# Load image
image_path = 'path/to/crop_image.jpg'

# Analyze
results = analyzer.predict(image_path)

# Display results
print(f"🌾 Crop Type: {results['crop_type']}")
print(f"🦠 Disease: {results['disease']}")
print(f"📊 Confidence: {results['confidence']:.2%}")
print(f"💊 Treatment: {results['treatment']}")
```

**Example 2: Web Interface**
```bash
streamlit run app.py
# Open browser and upload image through the UI
```

### 3️⃣ **Interpret Results**

| Result | Meaning |
|--------|---------|
| ✅ **Healthy** | No disease detected - Continue regular care |
| ⚠️ **Warning** | Early signs detected - Monitor closely |
| 🔴 **Alert** | Disease confirmed - Apply recommended treatment |

### 4️⃣ **Get Recommendations**

Results include:
- 📋 **Disease Name & Description**
- 📊 **Severity Level** (1-10 scale)
- 🌱 **Organic Treatment Options**
- 💊 **Chemical Treatment Options**
- 🚜 **Prevention Methods**
- 📚 **Reference Links**

---

## 🔧 Technologies Used

| Technology | Purpose |
|-----------|---------|
| 🧠 **TensorFlow/Keras** | Deep learning models |
| 🖼️ **OpenCV** | Image processing |
| 🔢 **NumPy/Pandas** | Data handling |
| 📊 **Matplotlib/Seaborn** | Visualization |
| 🌐 **Streamlit** | Web interface |
| 🚀 **Jupyter Notebook** | Development & documentation |

---

## 🎯 Example Outputs

### Success Case ✅

```
════════════════════════════════════════
        🌾 CROP ANALYSIS REPORT 🌾
════════════════════════════════════════
📍 Crop Type:        Tomato
🦠 Disease Status:   HEALTHY ✅
📊 Confidence:       98.5%
❤️ Health Score:      9.5/10

💡 Recommendations:
   ✓ Continue regular watering schedule
   ✓ Monitor for early signs of disease
   ✓ Maintain proper fertilization
════════════════════════════════════════
```

### Disease Detection Case ⚠️

```
════════════════════════════════════════
        🌾 CROP ANALYSIS REPORT 🌾
════════════════════════════════════════
📍 Crop Type:        Wheat
🦠 Disease:          Powdery Mildew ⚠️
📊 Confidence:       94.2%
❤️ Health Score:      5.8/10
🔴 Severity:         MEDIUM

💊 Treatment Options:
   
   Organic:
   • Spray baking soda solution (1 tbsp per gallon)
   • Apply sulfur dust
   • Improve air circulation
   
   Chemical:
   • Use fungicide (e.g., Triazole)
   • Follow label instructions
   • Repeat every 7-10 days

🛡️ Prevention:
   • Avoid overhead watering
   • Maintain proper spacing
   • Remove infected leaves
   
════════════════════════════════════════
```

---

## 🤝 Contributing

We welcome contributions! Here's how you can help:

### 🐛 Report Issues
Found a bug? Create an issue with:
- 📝 Clear description
- 📸 Screenshots/images
- 🔧 Steps to reproduce

### 🌟 Suggest Features
Have an idea? Open a feature request!

### 👨‍💻 Submit Code Changes
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit changes (`git commit -m 'Add amazing feature'`)
4. Push to branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📞 Support & Contact

- 🐛 **Issues**: [GitHub Issues](https://github.com/Jyotirjay37/Crop_Care/issues)
- 💬 **Discussions**: [GitHub Discussions](https://github.com/Jyotirjay37/Crop_Care/discussions)
- 👤 **Author**: [@Jyotirjay37](https://github.com/Jyotirjay37)

---

## ⭐ Show Your Support

If you find this project helpful, please consider:
- ⭐ **Starring** this repository
- 🔀 **Forking** and contributing
- 📢 **Sharing** with your network
- 💬 **Providing feedback**

```
   🌾 Happy Farming! 🚜
```

---

<div align="center">

**Made with ❤️ for sustainable agriculture**

*Last Updated: June 2026*

</div>
