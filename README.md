# HaoroShi-Deeptection 🔍
A real-time deepfake detection browser extension powered by a hybrid CNN-Transformer architecture. Haoroshi Deeptection uses advanced machine learning to analyze images and videos directly in your browser, helping identify manipulated media content.

## 📑 Table of Contents
- 🌟 Features
- 🚀 Quick Start
- 📦 Installation
- 💡 Usage
- 🔬 How It Works
- 🏗️ Model Architecture
- 📊 Training Details
- 📈 Performance
- 🛠️ Development
- 🙏 Acknowledgments

## 📑 Table of Contents
- [🌟 Features](#features)
- [🚀 Quick Start](#quick-start)
- [📦 Installation](#installation)
- [💡 Usage](#usage)
- [🔬 How It Works](#how-it-works)
- [🏗️ Model Architecture](#model-architecture)
- [📊 Training Details](#training-details)
- [📈 Performance](#performance)
- [🛠️ Development](#development)
- [🙏 Acknowledgments](#acknowledgments)

## 🌟 Features
- **Real-time Detection**: Analyze images and videos directly in your browser
- **Triple Mode Operation**:
  - 🌐 **Webpage Mode**: Analyzes images embedded in web pages (source images)
  - 📸 **Screenshot Mode**: Captures and analyses screen snapshots
  - 🎥 **Video Mode**: Processes video content frame-by-frame
- **Advanced AI Model**: Hybrid CNN-Transformer architecture combining local and global feature analysis
- **Privacy-First**: All processing happens locally in your browser
- **Toggleable Interface**: Easy-to-use movable overlay that can be activated/deactivated
- **PDF Reports**: Generate detailed analysis reports with confidence scores

## 🚀 Quick Start
Get started with HaoroShi Deeptection in 3 simple steps:
1. **Download** the extension files from this repository
2. **Load** the extension in your browser (see [Installation](#-installation) for browser-specific steps)
3. **Activate** by clicking the extension icon and start analyzing!


## 📦 Installation
### Pre-Requisites
- A Chromium-based browser (Chrome, Edge, Brave)
- Download or clone this repository to your computer
- 
### Step 1: Download the Extension
```bash
# Option 1: Clone the repository
git clone https://github.com/yourusername/haoroshi-deeptection.git

# Option 2: Download ZIP
# Click "Code" → "Download ZIP" on GitHub, then extract
```

### Step 2: Load the Extension in Your Browser

Choose your browser and follow the steps:

<details>
<summary><b>🔵 Google Chrome</b></summary>

1. Open Chrome and navigate to `chrome://extensions/`:

   <img width="950" alt="Chrome Extensions Page" src="https://github.com/user-attachments/assets/f5cfb2a7-6ab7-4e1e-96e4-5deb044bbf26" />

2. Enable **Developer mode** (toggle in top-right corner):

   <img width="1920" alt="Enable Developer Mode" src="https://github.com/user-attachments/assets/31ca84bd-7a7e-4e14-8e36-9fff03b3c3ae" />

3. Click **"Load unpacked"**:

   <img width="1920" alt="Load Unpacked Button" src="https://github.com/user-attachments/assets/30a39492-27d9-4486-a94c-cec4cadb8d6a" />

4. Navigate to the `haoroshi-deeptection` folder, then select the **`dist`** folder:

   <img width="1920" alt="Select dist folder" src="https://github.com/user-attachments/assets/cf3995cd-c3b8-436c-9c52-560f3bef40a0" />

5. The extension should now be loaded! The icon will appear in your toolbar ✅

   <img width="952" alt="Extension loaded successfully" src="https://github.com/user-attachments/assets/6aee2ace-e02d-4ab5-a55e-068dbeccee0e" />

</details>

<details>
<summary><b>🔷 Microsoft Edge</b></summary>

1. Open Edge and navigate to:
```
   edge://extensions/
```
2. Enable **Developer mode** (toggle in left sidebar)
3. Click **"Load unpacked"**
4. Select the `haoroshi-deeptection` folder
5. The extension icon should appear in your toolbar ✅

</details>

<details>
<summary><b>🦁 Brave Browser</b></summary>

1. Open Brave and navigate to:
```
   brave://extensions/
```
2. Enable **Developer mode** (toggle in top-right corner)
3. Click **"Load unpacked"**
4. Select the `haoroshi-deeptection` folder
5. The extension icon should appear in your toolbar ✅

</details>

<details>
<summary><b>🦊 Mozilla Firefox</b></summary>

1. Open Firefox and navigate to:
```
   about:debugging#/runtime/this-firefox
```
2. Click **"Load Temporary Add-on..."**
3. Navigate to the `haoroshi-deeptection` folder
4. Select the `manifest.json` file
5. The extension icon should appear in your toolbar ✅

> **Note**: In Firefox, temporary extensions are removed when you close the browser. For permanent installation, you'll need to package and sign the extension.

</details>

### Step 3: Verify Installation

✅ You should see the HaoroShi Deeptection icon in your browser toolbar  
✅ Click the icon to activate/deactivate the extension  
✅ A movable overlay should appear on any webpage when activated

> **Note**: If the icon doesn't appear, click the puzzle piece icon (🧩) in your toolbar to pin the extension.


## 💡 Usage

## 🔬 How It Works


## 🏗️ Model Architecture
Model Architecture
The deepfake detection model uses a hybrid CNN-Transformer architecture:

**Key Components:**
- CNN Backbone: EfficientNet-B0 (pretrained on ImageNet) for efficient local feature extraction
- Transformer Encoder: 6-layer transformer with multi-head self-attention for capturing global dependencies
- Multi-Task Learning: Dual heads for classification and artifact detection
- Total Parameters: ~87M parameters

## 📊 Training Details

## 📈 Performance

## Acknowledgement
