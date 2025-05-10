# 👕 VirtuWear

**VirtuWear** is a real-time virtual try-on application that allows users to wear digital clothing (like T-shirts) through their webcam feed or uploaded images. Built using advanced computer vision and deep learning, the system uses **YOLOv8 Pose Estimation** to detect body keypoints and overlays virtual clothing with realistic positioning and scale.

---

## 🚀 Features

- 🔍 **YOLOv8 Pose Detection**: Real-time upper-body keypoint detection (shoulders, elbows, waist).
- 🧠 **Intelligent Augmentation**: Dynamically scales and overlays clothing images using pose data.
- 🌐 **Web Interface**: Streamlit-powered UI for image or live video-based try-on.
- 🖼️ **Custom Clothing Support**: Annotate your own T-shirts using the built-in tool.
- 📦 **Modular Codebase**: Clearly separated modules for detection, augmentation, and streaming.

---

## 🛠️ Tech Stack

| Technology        | Purpose                                |
|-------------------|----------------------------------------|
| **Python 3.9+**    | Core programming language              |
| **OpenCV**         | Image and video processing             |
| **YOLOv8**         | Human pose estimation                  |
| **Ultralytics**    | Pre-trained pose models integration    |
| **NumPy**          | Array operations and data manipulation |
| **Streamlit**      | Web-based UI for interaction           |
| **PyTorch**        | Deep learning framework for YOLOv8     |

---


---

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/VirtuWear.git
cd VirtuWear
````
### 2. Create and Activate Virtual Environment
````bash
conda create --name tryon-env python=3.9
conda activate tryon-env
````
### 3. Install dependencies
````bash
# Install PyTorch (adjust CUDA version as needed)
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118

# Install other packages
pip install ultralytics opencv-python streamlit numpy
````
### 🧪 How to Run the App
Launch the Streamlit Interface
````bash
streamlit run webapp.py
````
* This will open a browser window at http://localhost:8501.

* Use your webcam to see real-time pose detection and try on the virtual shirt.

### 🖍️ Annotate Your Own T-Shirt
To annotate custom T-shirt keypoints:
```bash
python annotate_shirts.py
````
* Input the absolute path to the image when prompted.

* Double-click to mark up to 4 keypoints on the shirt image.

* Press q to save the annotation and overwrite the image.

⚠️ Ensure your clothing image has a transparent background (PNG) for best results.



**📄 License**

This project is licensed under the MIT License.


**🙏 Acknowledgements**

* Ultralytics YOLOv8

* Streamlit

* OpenCV



