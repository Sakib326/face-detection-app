# Live Face Detection and Registration System

This is a web-based face detection and registration system using **face-api.js**. It allows real-time face detection, registration, and recognition directly in the browser.

---

## Features

- Real-time face detection and recognition.
- Face registration with user-provided names.
- Displays age, gender, and expressions of detected faces.
- Lightweight and runs entirely in the browser without requiring a backend.

---

## Installation Guide

### **1. Prerequisites**

Ensure the following tools are installed:

- **Node.js** ([Download Node.js](https://nodejs.org/))
- **npm** (Comes with Node.js)
- **http-server** or **live-server**

### **2. Setup the Project**

1. Clone this repository or download the source code.

   ```bash
   git clone <repository-url>
   cd face-detection-app
   ```

2. Create a folder named **models** inside the project directory.
3. Download the pre-trained models from the **face-api.js** repository:
   [Download Models](https://github.com/justadudewhohacks/face-api.js/tree/master/weights)
4. Place the downloaded model files inside the **models** folder.

### **3. Install HTTP Server**

You need a local server to serve the HTML file since camera access requires a secure context.

#### Option 1: Using Node.js and http-server

1. Install **http-server** globally:
   ```bash
   npm install -g http-server
   ```
2. Start the server in your project directory:
   ```bash
   http-server
   ```
3. Open the provided URL (e.g., `http://localhost:8080`) in your browser.

#### Option 2: Using Live Server (VS Code Extension)

1. Install **Live Server** extension in Visual Studio Code.
2. Open the project folder in VS Code.
3. Right-click on **index.html** → Select **Open with Live Server**.

#### Option 3: Using Python (Optional)

For Python 3:

```bash
python -m http.server 8000
```

For Python 2:

```bash
python -m SimpleHTTPServer 8000
```

Visit: `http://localhost:8000`

---

## Usage

1. Open the application in your browser.
2. Allow camera permissions when prompted.
3. Enter a name in the input box and click **Register Face** to add a face.
4. Faces will be detected in real time with age, gender, and expressions displayed.
5. Click **Clear All Faces** to reset registrations.

---

## File Structure

```
face-detection-app/
|-- index.html
|-- models/
|   |-- faceLandmark68Net-weights_manifest.json
|   |-- ssdMobilenetv1_model-weights_manifest.json
|-- README.md
```

---

## Troubleshooting

1. **Models not loading:**
   - Ensure models are in the `models/` folder and accessible.
2. **Webcam not working:**
   - Check browser permissions and refresh the page.
3. **Errors in Console:**
   - Open DevTools (F12) → Console for debugging.

---

## Dependencies

- **face-api.js** - Facial recognition library.
- **http-server** or **live-server** - Local server.

---

## License

This project is open-source and available under the **MIT License**.

---

## Credits

Developed using **face-api.js** by [justadudewhohacks](https://github.com/justadudewhohacks).
