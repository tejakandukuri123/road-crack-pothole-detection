# Road Crack & Pothole Detection System

An image-based road defect detection system developed using Python and image processing techniques to identify and visualize road cracks and potholes from road images.

## Features

- Upload road images for analysis
- Detect potential road defects using local entropy analysis
- Percentile-based thresholding for defect identification
- Morphological image processing for noise removal and region refinement
- Filters small regions and potential lane markings
- Detects and classifies regions as Deep or Medium severity
- Draws bounding boxes around detected defects
- Displays defect counts
- Configurable detection parameters
- Download processed detection results

## Technologies Used

- Python
- OpenCV
- NumPy
- Scikit-image
- Flask
- HTML
- Bootstrap

## Image Processing Pipeline

1. Upload a road image through the web interface.
2. Convert the image to grayscale.
3. Calculate local entropy to identify areas with significant texture variation.
4. Apply percentile-based thresholds to generate Deep and Medium detection masks.
5. Apply morphological operations to clean the masks.
6. Remove small regions and potential lane markings.
7. Analyze connected regions and generate bounding boxes.
8. Display the processed image along with Deep and Medium defect counts.

## Project Structure

```text
road-crack-pothole-detection/
│
├── app.py
├── requirements.txt
│
└── templates/
    └── index.html
