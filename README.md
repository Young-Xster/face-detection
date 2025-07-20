# Face Detection Project

A Python project for real-time face detection using OpenCV and Haar Cascades.

## Features

- **Real-time face detection** from webcam feed
- **Haar Cascade classifier** for accurate face detection
- **turquoise bounding boxes** around detected faces
- **Easy to extend** for additional features
- **Clean, simple code** structure

## Setup

### Prerequisites

- Python 3.12+
- Webcam (for real-time detection)

### Installation

1. Clone the repository:

```bash
git clone https://github.com/Young-Xster/face-detection.git
cd face-detection
```

2. Create and activate virtual environment:

```bash
python -m venv .venv
source .venv/bin/activate  # Linux/Mac
# or
.venv\Scripts\activate     # Windows
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

## Usage

### Running the Face Detection

**Option 1: Using VS Code**

- Set Python interpreter to `.venv` environment
- Click the ▶️ Run button

**Option 2: Using Terminal**

```bash
# Activate virtual environment first
source .venv/bin/activate
python face_detection.py
```

**Option 3: Direct execution**

```bash
.venv/bin/python face_detection.py
```

### Controls

- **Press 'q'** to quit the application

### Using Video File Instead of Webcam

Uncomment line 11 in `face_detection.py` and replace `"video.mp4"` with your video file path:

```python
# camera = cv2.VideoCapture(0)  # Comment this line
video = cv2.VideoCapture("your_video.mp4")  # Uncomment and modify this line
```

## Technical Details

- **Haar Cascade**: Uses OpenCV's pre-trained frontalface cascade
- **Detection Parameters**:
  - Scale Factor: 1.1
  - Min Neighbors: 5
  - Min Size: 30x30 pixels
- **Color Space**: Converts to grayscale for detection
- **Bounding Box**: Yellow rectangles (BGR: 255, 255, 0)

## Dependencies

- `opencv-python` - Computer vision library
- `numpy` - Numerical computations
- `matplotlib` - Plotting library
- `Pillow` - Image processing

## Next Steps

- [ ] Add face recognition capabilities
- [ ] Implement multiple face detection algorithms
- [ ] Add face landmark detection
- [ ] Create GUI interface
- [ ] Add image file processing
- [ ] Implement face tracking
- [ ] Add face blur/anonymization features
