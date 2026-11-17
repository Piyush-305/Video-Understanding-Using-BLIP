#  Video Understanding Using BLIP 🤖

### 🚀 Turning Video Frames into AI-Generated Captions!

<p align="center">

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python&logoColor=white)
![BLIP](https://img.shields.io/badge/AI-BLIP-orange?style=for-the-badge)
![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-red?style=for-the-badge&logo=pytorch&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-green?style=for-the-badge&logo=opencv&logoColor=white)

</p>

---

## 🌟 About The Project

Ever wondered how Artificial Intelligence can describe the contents of a video?

**Video Understanding Using BLIP** is a Python-based Computer Vision project that extracts selected frames from a video, combines them into a visual grid, and uses a pretrained BLIP (Bootstrapping Language-Image Pretraining) model to generate natural-language descriptions.

Instead of manually describing video content, the system uses AI to analyze visual information and produce an automatic caption.

💡 This project combines video processing, image analysis, and deep learning in a single pipeline.

## ✨ Key Features

- 🎬 **Video Processing:** Reads and processes video files using OpenCV.
- 🖼️ **Frame Extraction:** Extracts individual frames from video input.
- 🎯 **Frame Sampling:** Selects four evenly distributed frames.
- 🔲 **Temporal Grid Generation:** Combines selected frames into a single image.
- 🧠 **AI-Powered Captioning:** Uses the BLIP pretrained model to generate captions.
- ⚡ **Local AI Inference:** Runs the model locally using PyTorch.
- 🔐 **No API Key Required:** No paid AI API or API credentials are needed.
- 📁 **Output Generation:** Saves the processed frame grid for inspection.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| 🐍 Python | Core programming language |
| 👁️ OpenCV | Video reading and frame extraction |
| 🔢 NumPy | Numerical operations and frame sampling |
| 🖼️ Pillow | Image processing |
| 🔥 PyTorch | Deep learning inference |
| 🤗 Transformers | Pretrained model integration |
| 🧠 BLIP | Image caption generation |

## ⚙️ How It Works

The project follows this AI-powered processing pipeline:

```text
       🎥 VIDEO INPUT
             |
             ▼
        👁️ OpenCV
       Video Loading
             |
             ▼
      🖼️ Frame Extraction
             |
             ▼
       🎯 Frame Sampling
         (4 Frames)
             |
             ▼
       🔲 Temporal Grid
          (2 × 2)
             |
             ▼
        🧠 BLIP MODEL
       Image Captioning
             |
             ▼
      💬 GENERATED CAPTION
```

### 🔍 Processing Steps

**1️⃣ Video Input**

The system reads a video using OpenCV. By default, the program generates a synthetic sample video containing a moving red circle and a blue rectangle.

**2️⃣ Frame Extraction**

Individual frames are extracted and converted from BGR to RGB format.

**3️⃣ Frame Sampling**

Four frames are selected at evenly spaced intervals to represent different portions of the video.

**4️⃣ Temporal Grid Creation**

The selected frames are resized and combined into one 2 × 2 image grid.

**5️⃣ AI Caption Generation**

The combined image is passed to the pretrained BLIP model, which analyzes its visual contents and generates a natural-language caption.

**6️⃣ Final Output**

The generated caption is displayed in the terminal, while the processed frame grid is saved as an image.

## 🧠 AI Model Information

| Detail | Information |
|---|---|
| Model | BLIP Image Captioning Base |
| Model Name | `Salesforce/blip-image-captioning-base` |
| Model Provider | Salesforce |
| Platform | Hugging Face |
| Framework | PyTorch |

🔗 **[Explore the BLIP pretrained model](https://huggingface.co/Salesforce/blip-image-captioning-base)**

BLIP is a Vision-Language Model designed to connect visual information with natural language. In this project, it performs image captioning on a combined image of sampled video frames.

## 📂 Project Structure

```text
Video-Understanding-Using-BLIP/
│
├── main.py
├── requirements.txt
│
└── outputs/
```

| File | Description |
|---|---|
| `main.py` | Main Python program |
| `requirements.txt` | Required Python libraries |
| `outputs/` | Directory for sample output images |

## 🚀 Getting Started

### 📋 Prerequisites

- Python 3.9 or later (subject to dependency compatibility).
- Internet connection for the initial model download.
- Sufficient memory and storage for PyTorch and BLIP.

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/Piyush-305/Video-Understanding-Using-BLIP
```

### 2️⃣ Navigate to the Project

```bash
cd Video-Understanding-Using-BLIP
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Run the Project

```bash
python main.py
```

The pretrained BLIP model will be downloaded during its first execution if it is not already available locally.

## 💻 Offline Functionality

🌐 **First Execution:** An internet connection is required to download the pretrained BLIP model and its required files.

💻 **Subsequent Executions:** Once the model and dependencies are installed, video processing and caption generation can run locally without an internet connection.

🔐 No API key or paid cloud inference service is required.

## 📸 Expected Outputs

The project produces the following outputs:

| Output | Description |
|---|---|
| `sample_video.avi` | Generated synthetic sample video |
| `debug_grid.jpg` <img width="448" height="448" alt="debug_grid" src="https://github.com/user-attachments/assets/a10a89fc-d0cf-4529-95f1-07a8d5bcdf18" />
| Combined image of four sampled frames |
| Terminal Caption | AI-generated visual description |

**Example caption (illustrative):**

> 📝 A red circle and a blue square.

*Actual captions depend on the model's interpretation of the image.*

## ⚠️ Current Limitations

- The current implementation samples only four frames.
- BLIP is an image-captioning model, not a dedicated video-understanding model.
- The combined image does not provide true temporal or motion understanding.
- Events occurring between sampled frames may be missed.
- Caption accuracy depends on the selected frames and their visual quality.

## 🔮 Future Enhancements

- 🎞️ Dynamic video selection.
- 🖼️ Extraction and analysis of more frames.
- 📝 Individual captions for multiple frames.
- 📚 Comprehensive video summarization.
- 🏃 Improved activity and event recognition.
- 🤖 Integration of advanced video-language models.
- 🖥️ Development of a user-friendly graphical interface.

## 🎯 Project Objective

The primary objective is to explore how Computer Vision and Vision-Language Models can be combined to automate visual content description.

This project demonstrates the integration of video processing techniques with pretrained deep learning models for AI-based caption generation.

---

## ⭐ Support

If you find this project interesting, consider giving the repository a ⭐!

**🚀 Exploring the intersection of Computer Vision and Artificial Intelligence!**
