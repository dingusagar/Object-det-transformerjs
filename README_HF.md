---
title: Real-time Object Detection
emoji: 🤖
colorFrom: blue
colorTo: purple
sdk: static
pinned: false
license: mit
---

# 🤖 Real-time Object Detection

A modern web application for real-time object detection using **Transformers.js** and **YOLOv9**. This project runs entirely in your browser with AI-powered computer vision - no server required!

## ✨ Features

- 🎥 **Real-time webcam object detection**
- 🧠 **Multiple YOLO models** (YOLO Tiny, Small, YOLOv9, GELAN-C)
- ⚡ **Browser-based AI** - runs locally without server
- 🎨 **Modern glassmorphism UI** with dark mode
- 🎛️ **Adjustable parameters** (threshold, image size, scale)
- 📱 **Responsive design** for all devices

## 🎮 How to Use

1. **Allow webcam access** when prompted by your browser
2. **Select a model** from the dropdown menu:
   - **YOLO Tiny** - Fastest, best for low-end devices
   - **YOLO Small** - Balanced performance
   - **YOLOv9 Compact** - Higher accuracy
   - **GELAN-C** - Recommended for best results
3. **Click "Load Model"** - First load will download the model (cached for future use)
4. **Adjust parameters** using the sliders for optimal detection
5. **Watch real-time detections** appear as bounding boxes!

## 🛠️ Tech Stack

- **[Transformers.js](https://huggingface.co/docs/transformers.js)** - Run ML models in the browser
- **[YOLOv9](https://github.com/WongKinYiu/yolov9)** - State-of-the-art object detection
- **[Vite](https://vitejs.dev/)** - Fast build tool
- **Vanilla JavaScript** - No framework overhead

## 📦 Local Development

```bash
git clone https://github.com/dingusagar/Object-det-transformerjs.git
cd Object-det-transformerjs
npm install
npm run dev
```

## 📄 License

MIT License - Created by [@dingusagar](https://github.com/dingusagar)

---

⭐ If you found this project helpful, please give it a star on [GitHub](https://github.com/dingusagar/Object-det-transformerjs)!
