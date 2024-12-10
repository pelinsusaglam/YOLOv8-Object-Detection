# YOLOv8-Object-Detection

This script performs object detection on an image using the YOLOv8 model. It reads an image, runs the YOLOv8 object detection model on it, and draws bounding boxes around detected objects with their class names and confidence scores.

## Features
- Loads an image from the specified path.
- Runs object detection using the YOLOv8 model.
- Draws bounding boxes around detected objects.
- Displays the class names and confidence scores for each detected object.

## How It Works
1. **Load Image:** The script loads an image (`bus.jpg`) from the specified path and resizes it for easier processing.
2. **Object Detection:** YOLOv8 is used to detect objects in the image.
   - If the detection confidence score is above a threshold (default is 0.5), a bounding box is drawn around the object.
   - The object class name and confidence score are displayed above the bounding box.
3. **Display the Result:** The processed image with bounding boxes and labels is shown using `cv2_imshow`.

## Requirements
- Python 3.7+
- OpenCV
- Imutils
- Ultralytics YOLO
- Google Colab (for `cv2_imshow`)

## How to Use
1. Make sure the YOLOv8 model (`yolov8n.pt`) and the image (`bus.jpg`) are placed in the correct directory or update the `img_path` and `model_path` in the script.
2. Run the script to perform object detection on the image.
3. The processed image with bounding boxes and labels will be displayed.

## Output
- **Processed Image:** The image with bounding boxes drawn around detected objects, with the class name and confidence score displayed above each box.
