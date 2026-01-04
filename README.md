# HaoroShi-Deeptection 🔍
A real-time deepfake detection browser extension powered by a hybrid CNN-Transformer architecture. Haoroshi Deeptection uses advanced machine learning to analyse images and videos directly in your browser, helping identify manipulated media content.

## 📑 Table of Contents

- [🌟 Features](#-features)
- [🚀 Quick Start](#-quick-start)
- [📦 Installation](#-installation)
- [💡 Usage](#-usage)
- [📊 Statistics & Analytics](#-statistics--analytics)
- [🔬 How It Works](#-how-it-works)
- [🏗️ Model Architecture](#-model-architecture)
- [📊 Training Details](#-training-details)
- [📈 Performance](#-performance)
- [🙏 Acknowledgments](#-acknowledgments)
  
## 🌟 Features
- **Real-time Detection**: Analyse images and videos directly in your browser
- **Triple Mode Operation**:
  - 🌐 **Webpage Mode**: Analyses images embedded in web pages (source images)
  - 📸 **Screenshot Mode**: Captures and analyses screen snapshots
  - 🎥 **Video Mode**: Processes video content frame-by-frame
- **Intergrated DL Model**: Hybrid CNN-Transformer architecture combining local and global feature analysis
- **Privacy-First**: All processing happens locally in your browser
- **Toggleable Interface**: Easy-to-use movable overlay that can be activated/deactivated
- **PDF Reports**: Generate detailed analysis reports with confidence scores
- **Statistics & Analytics**: Track your scanning history with detailed metrics
  - View total scans, fake/real detection counts
  - Monitor fake rate percentage
  - Time-range filtering (day, week, month, year)
  - Visual charts showing detection trends
- **Feedback System**: Provide corrections and confirmations on detection results
  - Help improve the model accuracy
  - Review your feedback history
  - Export data for analysis

## 🚀 Quick Start
Get started with HaoroShi Deeptection in 3 simple steps:
1. **Download** the extension files from this repository
2. **Load** the extension in your browser (see [Installation](#-installation) for browser-specific steps)
3. **Activate** by clicking the extension icon and start analysing!


## 📦 Installation
### Prerequisites
- A supported browser: Chrome, Edge, Brave, or Firefox
- No additional software required

### Step 1: Download the Extension

1. Go to the [**Releases**](https://github.com/yourusername/haoroshi-deeptection/releases) page
<img width="1920" height="1080" alt="11" src="https://github.com/user-attachments/assets/a1b855b2-5fc8-439b-a586-1c81369992d1" />
<img width="1920" height="1080" alt="12" src="https://github.com/user-attachments/assets/c6658add-c732-4858-8f34-da5f0755a001" />
2. Download the **latest release** (`.zip` file)
3. Extract the downloaded ZIP file to a folder on your computer
<img width="1920" height="1080" alt="13" src="https://github.com/user-attachments/assets/69bb8402-038d-47b9-b1d5-3a7b21aeb409" />

> **💡 Tip**: Extract to a permanent location (e.g., `Documents/Extensions/HaoroShi-Deeptection`) as the extension needs to stay in this folder to work.

**Alternative: Clone the Repository** (For Developers)
```bash
# Download ZIP
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
<img width="1920" height="1080" alt="Step 1" src="https://github.com/user-attachments/assets/d52aa3f7-11ff-4e16-88be-378837cb1a5d" />

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
<img width="1920" height="1080" alt="5" src="https://github.com/user-attachments/assets/eb89a6da-d90f-42f2-adaf-c19f7b059296" />

3. Click **"Load unpacked"**
<img width="1920" height="1080" alt="6" src="https://github.com/user-attachments/assets/1d8b6e94-a7b8-4d62-9a5b-a8b04d0394ab" />

4. Select the `haoroshi-deeptection` folder
<img width="1920" height="1080" alt="Step 1" src="https://github.com/user-attachments/assets/fdbefd0c-6350-4203-93ff-b25107a68e56" />

5. The extension icon should appear in your toolbar ✅
<img width="1920" height="1080" alt="7" src="https://github.com/user-attachments/assets/838dab7b-f74b-4060-8295-1f496b8d4946" />

</details>

<details>
<summary><b>🦁 Brave Browser</b></summary>

1. Open Brave and navigate to:
```
   brave://extensions/
```
2. Enable **Developer mode** (toggle in top-right corner)
<img width="1920" height="1080" alt="8" src="https://github.com/user-attachments/assets/f2d79362-3436-4ce5-98e1-f057773d5132" />

3. Click **"Load unpacked"**
<img width="1920" height="1080" alt="9" src="https://github.com/user-attachments/assets/8770cd10-7a89-4d73-b4fb-c032f13b550d" />

4. Select the `haoroshi-deeptection` folder
<img width="1920" height="1080" alt="Step 1" src="https://github.com/user-attachments/assets/04abf66c-d4d7-4bbe-b93e-0fc287cede7f" />

5. The extension icon should appear in your toolbar ✅
<img width="1920" height="1080" alt="10" src="https://github.com/user-attachments/assets/565c4f5e-81d3-47fd-8f18-a5100a6a80ac" />
</details>

### Step 3: Verify Installation
✅ You should see the HaoroShi Deeptection icon in your browser toolbar  
✅ Click the icon to activate/deactivate the extension  
<img width="956" height="688" alt="image" src="https://github.com/user-attachments/assets/6d010894-a9f6-4665-918e-85dee96fefaf" />
✅ A movable overlay should appear on any webpage when activated
<img width="956" height="469" alt="image" src="https://github.com/user-attachments/assets/3c35e667-7c89-485d-98c8-97007a25c029" />

> **Note**: If the icon doesn't appear, click the puzzle piece icon (🧩) in your toolbar to pin the extension.


## 💡 Usage
1. **Activate the Extension**
   - Click the HaoroShi Deeptection icon in your browser toolbar
   - The movable overlay will appear on your current page
   - You can drag it to any position on the screen

2. **Select Detection Mode**
   The extension offers three analysis modes:

   #### 🌐 Webpage Mode
   - Automatically scans all images on the current webpage
   - Detects images from page source (HTML `<img>` tags)
   - Click "Analyse Page" to scan all images
   - Results show for each detected image

   #### 📸 Screenshot Mode
   - Captures the visible portion of your screen
   - Useful for analysing content in videos, apps, or protected images
   - Click "Capture Screenshot" button
   - The screenshot is analysed immediately

   #### 🎥 Video Mode
   - Analyses video content frame-by-frame
   - Works with embedded videos (YouTube, social media, etc.)
   - Click "Analyse Video" to start
   - Real-time analysis as the video plays

3. **Interpret Results**
   For each analysis, you'll see:
   - **Confidence Score**: Percentage indicating Real vs. Fake
   - **Classification**: 
     - 🟢 **REAL** - Likely authentic (green)
     - 🔴 **FAKE** - Likely manipulated (red)
     - 🟡 **UNCERTAIN** - Low confidence (yellow)
   - **Artifact Score**: Detection of manipulation artifacts
   - **Processing Time**: How long the analysis took

4. **Provide Feedback** (Optional)
   - If you believe the detection is incorrect, click "Provide Feedback"
   - Choose:
     - ✅ **Confirm**: The detection was correct
     - ❌ **Correct**: The detection was wrong (provide the correct label)
   - Your feedback helps improve accuracy

5. **View Statistics**
   - Click the extension icon and navigate to "Statistics & Feedbacks"
   - View your scanning history:
     - **Total Scans**: Number of analyses performed
     - **Total Images/Videos**: Breakdown by content type
     - **Fake Detections**: How many fakes were detected
     - **Real Detections**: How many real images were detected
     - **Fake Rate**: Percentage of scans that were fake
   - Filter by time range (Today, This Week, This Month, Whole Year)
   - View visual charts showing detection trends over time

6. **Manage Your Data**
   - **Export Data**: Download your statistics and feedback history
   - **Clear Stats**: Reset your scan statistics
   - **Clear Feedbacks**: Remove all feedback history
   - **Clear All Data**: Complete data reset
  
## 📊 Statistics & Analytics
<img width="1577" height="896" alt="image" src="https://github.com/user-attachments/assets/c18979bd-fdf3-415c-b17a-8cd499693cb7" />

HaoroShi Deeptection tracks your usage to help you understand your scanning patterns:
### Scan Metrics
- **Total Scans**: Cumulative number of analyses
- **Content Type Breakdown**: Images vs. Videos analysed
- **Detection Results**: Real vs. Fake counts
- **Fake Rate**: Percentage of content detected as fake
- **Time-based Filtering**: View statistics by day, week, month, or year

### Feedback System
- **Confirmations**: Cases where you agreed with the detection
- **Corrections**: Cases where you provided the correct label
- **Export Feature**: Download your complete history as JSON/CSV

### Privacy Note
All statistics are stored **locally in your browser**. No data is sent to external servers. You can clear your history at any time using the "Clear All Data" button.

## 🔬 How It Works
HaoroShi Deeptection uses a sophisticated multi-step process to detect deepfakes:

### The Detection Pipeline
```
📸 Input (Image/Video)
    ↓
🔍 Face Detection
    ↓ (Isolate facial regions)
🧠 AI Analysis (CNN-Transformer)
    ↓ (Extract features & patterns)
📊 Classification
    ↓ (Real vs. Fake prediction)
✅ Results + Confidence Score
```

### Step-by-Step Explanation

1. **Input Capture**
   - Webpage Mode: Extracts images from HTML
   - Screenshot Mode: Captures visible screen area
   - Video Mode: Extracts frames from video stream

2. **Face Detection** (using face-api.js)
   - Identifies all faces in the image
   - Extracts facial landmarks (eyes, nose, mouth)
   - Normalises face orientation and size

3. **Feature Extraction** (CNN Backbone)
   - Uses EfficientNet to analyse local patterns
   - Detects texture anomalies, blending artifacts
   - Identifies unnatural skin textures, lighting inconsistencies

4. **Global Analysis** (Transformer)
   - Examines relationships between facial features
   - Detects temporal inconsistencies (in videos)
   - Identifies manipulation patterns across the entire face

5. **Artifact Detection**
   - Searches for common deepfake artifacts:
     - Unnatural blurring around face boundaries
     - Color inconsistencies
     - Compression artifacts in specific regions
     - Abnormal facial symmetry

6. **Classification & Scoring**
   - Combines all signals into a final prediction
   - Outputs confidence score (0-100%)
   - Classifies as Real, Fake, or Uncertain

### Limitations
⚠️ **Not 100% Accurate** - Use as a verification tool, not absolute proof  
⚠️ **Quality Dependent** - Works best with clear, high-resolution images  
⚠️ **Evolving Threats** - New deepfake techniques may bypass detection  
⚠️ **Context Matters** - Consider multiple factors when verifying media authenticity

## 🏗️ Model Architecture
Model Architecture
The deepfake detection model uses a hybrid CNN-Transformer architecture:

**Key Components:**
- CNN Backbone: EfficientNet-B0 (pretrained on ImageNet) for efficient local feature extraction
- Transformer Encoder: 6-layer transformer with multi-head self-attention for capturing global dependencies
- Multi-Task Learning: Dual heads for classification and artifact detection
- Total Parameters: ~87M parameters

## 📚 Training Details
### Image Detection Model (ImageModel.onnx)

**Dataset:**
- **Training Set**: 100,000 images
  - Celeb-DF v2: 50,000 images
  - JamieWithofs: 50,000 images
- **Validation Set**: 20,104 images
- **Test Set**: 10,103 images

**Training Configuration:**
- **Epochs**: 40
- **Batch Size**: 16
- **Learning Rate**: 8e-5 (AdamW optimizer)
- **Weight Decay**: 0.01
- **Augmentation**: Mixup, label smoothing (0.1)
- **Training Time**: ~22 hours (CUDA)

**Performance:**
- **Test Accuracy**: 94.24%
- **Best Validation Accuracy**: 96.30%
- **Precision**: Real 92.40%, Fake 96.23%
- **Recall**: Real 96.37%, Fake 92.13%

---

### Video Detection Model (VideoModel2.onnx)

**Training Configuration:**
- **Epochs**: 26
- **Optimizer**: AdamW
- **Learning Rate**: 7.07e-4 (adaptive)

**Performance:**
- **Validation Accuracy**: 84.93%
- **Validation F1-Score**: 84.93%
- **Training Accuracy**: 78.77%

**Note:** The video model processes frames sequentially to detect temporal inconsistencies and manipulation patterns across video sequences.

---

### Key Training Techniques (Both Models)
- Transfer learning with EfficientNet-B0 (ImageNet pretrained)
- Multi-task learning (classification + artifact detection)
- Data augmentation for robustness
- Label smoothing for regularisation

## 📈 Performance
### Image Detection (ImageModel.onnx)
- **Test Accuracy**: 94.24%
- **Validation Accuracy**: 96.30% (best)
- **Precision**: Real 92.40%, Fake 96.23%
- **Recall**: Real 96.37%, Fake 92.13%
- **F1-Score**: 94.24% (weighted average)
- **Dataset**: Evaluated on Celeb-DF v2 test set (10,103 images)

### Video Detection (VideoModel2.onnx)
- **Validation Accuracy**: 84.93%
- **Validation F1-Score**: 84.93%
- **Dataset**: Evaluated on video frame sequences

> **Note**: Performance may vary on different datasets and real-world content. The models perform best on high-quality, face-forward images/videos. Video detection analyses temporal patterns across frames, which can be more challenging than single-image detection.

## 🙏 Acknowledgments
This project utilises the following datasets, research contributions, and software tools:

**Datasets:**
- Li, Y., Yang, X., Sun, P., Qi, H., & Lyu, S. (2020). *Celeb-DF (v2): A large-scale challenging dataset for deepfake forensics* [Data set]. arXiv. https://arxiv.org/abs/1909.12962

- JamieWithofs. (n.d.). *JamieWithofs dataset* [Data set]. Hugging Face. https://huggingface.co/datasets/JamieWithofs

**Research Papers:**
- Tan, M., & Le, Q. V. (2019). EfficientNet: Rethinking model scaling for convolutional neural networks. *Proceedings of the 36th International Conference on Machine Learning*, 97, 6105-6114. http://proceedings.mlr.press/v97/tan19a.html

- Dosovitskiy, A., Beyer, L., Kolesnikov, A., Weissenborn, D., Zhai, X., Unterthiner, T., Dehghani, M., Minderer, M., Heigold, G., Gelly, S., Uszkoreit, J., & Houlsby, N. (2020). An image is worth 16x16 words: Transformers for image recognition at scale. *arXiv preprint*. https://arxiv.org/abs/2010.11929

**Software:**
- Microsoft. (n.d.). *ONNX Runtime Web* [Computer software]. ONNX Runtime. https://onnxruntime.ai/docs/tutorials/web/

