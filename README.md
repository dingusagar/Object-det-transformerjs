# 🤖 Real-time Object Detection

A modern web application for real-time object detection using **Transformers.js** and **YOLOv9**. This project runs entirely in your browser with AI-powered computer vision - no server required!

![Object Detection Demo](https://img.shields.io/badge/AI-Object%20Detection-blue)
![Transformers.js](https://img.shields.io/badge/Transformers.js-2.15.0-green)
![Vite](https://img.shields.io/badge/Vite-5.1.7-purple)

## ✨ Features

- 🎥 **Real-time webcam object detection**
- 🧠 **Multiple YOLO models** (YOLO Tiny, Small, YOLOv9, GELAN-C)
- ⚡ **Browser-based AI** - runs locally without server
- 🎨 **Modern glassmorphism UI** with dark mode
- 🎛️ **Adjustable parameters** (threshold, image size, scale)
- 📱 **Responsive design** for all devices

## 🚀 Quick Start

### Prerequisites

- **Node.js** (v14 or higher)
- **npm** (comes with Node.js)
- A modern web browser with webcam access

### Installation

1. **Clone the repository**
   ```bash
   git clone git@github.com:dingusagar/Object-det-transformerjs.git
   cd Object-det-transformerjs
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Run the development server**
   ```bash
   npm run dev
   ```

4. **Open in browser**
   - The app will automatically open at `http://localhost:5173`
   - If not, navigate to the URL shown in your terminal
   - Allow webcam access when prompted

## 🎮 Usage

1. **Select a model** from the dropdown menu:
   - **YOLO Tiny** - Fastest, best for low-end devices
   - **YOLO Small** - Balanced performance
   - **YOLOv9 Compact** - Higher accuracy
   - **GELAN-C** - Recommended for best results

2. **Click "Load Model"** - First load will download the model (cached for future use)

3. **Adjust parameters** using the sliders:
   - **Image Size** - Processing resolution (64-256px)
   - **Threshold** - Detection confidence (0.01-1.0)
   - **Image Scale** - Video feed scaling (0-1)

4. **Watch real-time detections** appear as bounding boxes on your video feed!

## 📦 Build for Production

```bash
npm run build
```

The optimized production build will be in the `dist/` folder.

To preview the production build:
```bash
npm run preview
```

## 🛠️ Tech Stack

- **[Vite](https://vitejs.dev/)** - Fast build tool and dev server
- **[Transformers.js](https://huggingface.co/docs/transformers.js)** - Run ML models in the browser
- **[YOLOv9](https://github.com/WongKinYiu/yolov9)** - State-of-the-art object detection
- **Vanilla JavaScript** - No framework overhead
- **CSS3** - Modern glassmorphism design

## 📁 Project Structure

```
object-det/
├── index.html          # Main HTML file
├── main.js            # Core application logic
├── style.css          # Styling and animations
├── package.json       # Dependencies and scripts
├── vite.config.js     # Vite configuration
└── README.md          # This file
```

## 🔧 Configuration

### Vite Configuration
The project uses Vite with custom headers to support SharedArrayBuffer (required for Transformers.js):

```javascript
// vite.config.js
export default {
  server: {
    headers: {
      'Cross-Origin-Opener-Policy': 'same-origin',
      'Cross-Origin-Embedder-Policy': 'require-corp',
    },
  },
}
```

## 🌐 Browser Compatibility

- ✅ Chrome/Edge (recommended)
- ✅ Firefox
- ✅ Safari (latest versions)
- ⚠️ Requires webcam access
- ⚠️ Requires SharedArrayBuffer support

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests

## 📄 License

MIT License - feel free to use this project for learning and development!

## 🙏 Acknowledgments

- [Hugging Face](https://huggingface.co/) for Transformers.js
- [YOLOv9](https://github.com/WongKinYiu/yolov9) for the object detection models
- [Vite](https://vitejs.dev/) for the amazing build tool

## 📧 Contact

Created by [@dingusagar](https://github.com/dingusagar)

---

⭐ If you found this project helpful, please give it a star!
