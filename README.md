
## 🧰 Features
- AI-powered **depth estimation** using advanced models.
- Image **upscaling** with state-of-the-art algorithms.
- Customizable **animations** and filters.
- Fast video rendering with support for **hardware acceleration** (e.g., NVENC).
- Easy-to-use **Gradio web interface**.

---

## 📦 Installation

### Prerequisites
Make sure you have the following installed before proceeding:
- [Python](https://www.python.org/) >= 3.9
- [Pip](https://pip.pypa.io/en/stable/installation/)




### Required Dependencies
The core dependencies used in this project include:

| Dependency        | Description |
|-------------------|-------------|
| `gradio`          | Web UI framework |
| `dotmap`          | Dot-accessible dictionaries |
| `attrs`           | Class construction with less boilerplate |
| `pillow`          | Image processing |
| `typer`           | CLI app creation |
| `tqdm`            | Progress bars |
| `numpy`           | Numerical operations |
| `opencv-python`   | Computer vision utilities |
| `torch`           | Deep learning framework |
| `transformers`    | HuggingFace Transformers library |
| `onnxruntime`     | ONNX model inference |
| `ffmpeg-python`   | FFmpeg wrapper |

You can install them all at once:
```bash
pip install gradio dotmap attrs pillow typer tqdm numpy opencv-python torch transformers onnxruntime ffmpeg-python
```

> Optional: For better performance, install CUDA-compatible versions of PyTorch if you're using an NVIDIA GPU.

---

## ⚙️ Usage

### Launch the Web Interface
Once everything is installed, simply run the main script:
```bash
python filename.py
```
This will start a Gradio web server. Open the link in your browser and begin exploring!

### Options
You can customize the behavior using command-line arguments:
```bash
--port       Specify a port number (default: auto)
--server     Host IP address (default: 0.0.0.0)
--share      Generate a public shareable link
--workers    Maximum concurrent renders
--open       Open in browser automatically
--turbo      Enable TurboPipe for faster rendering
--nvenc      Use NVENC hardware encoding
```

Example:
```bash
python DepthGradio.py --port 7860 --share --turbo --nvenc
```

---

## 🧪 Example Workflow

1. Upload an image.
2. Click **"Estimate"** to generate a depth map.
3. Optionally upscale the image using one of the available models.
4. Configure animation presets (Orbital, Zoom, etc.).
5. Adjust output settings like resolution, duration, and quality.
6. Click **"Render"** to generate your video!

