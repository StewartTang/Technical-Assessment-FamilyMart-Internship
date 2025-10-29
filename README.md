# Technical-Assessment-FamilyMart-Internship

# Task 1 - Car Counter
# Vehicle Detection and Counting using YOLO + SORT Tracker

## Overview
This project build a solution to count the number of cars passing through a given point using video footage.

----

## Approach

1. **Detection**  
   Each frame from the input video is processed using the **YOLO** model.  
   YOLO identifies objects such as cars, trucks, and buses by providing bounding box coordinates and confidence scores.

2. **Tracking**  
   The **SORT** algorithm tracks each detected vehicle across frames and assigns a unique ID to avoid double counting.

3. **Counting**  
   A virtual line is drawn vertically.  
   When the center of a vehicle crosses this line, the car counter is incremented by 1.

4. **Display**  
   The processed video is displayed (or saved) with bounding boxes, object IDs, and the live vehicle count overlayed on each frame.

---

## Technologies and Tools Used

| Tool / Library | Purpose |
|-----------------|----------|
| **Python 3** | Main programming language |
| **OpenCV** | Image and video processing |
| **Ultralytics YOLOv8** | Object detection |
| **SORT** | Object tracking across frames |
| **NumPy** | Numerical operations |
| **Google Colab** | Environment for execution |
| **ChatGPT** | AI tools to improve my works, debugging and understanding some logic such as calculating the speed of the car in the video, how sort algorithm works |
| **Youtube** | Researching |

---

## Steps to Reproduce

### 1. Clone or Download the repository of ultralyytics, filterpy and sort to use the model and algorithm
### 2. Create a method for initialisation of the model, video and tracker 
### 3. Create a method for detecting the vehicles in the videos with the list of informations given (x1, y1, x2, y2, c_score, class_id) and setting a confidence score to identify how confidence is that frame is. 
### 4. Create a method for tracking the speed of the vehicles of the video using SORT and calculating center position of the car. If the car was detected previsouly compute the dstance between the old and new position. Finally, calculate the speed by multiplying fps and 3.6 to convert m/s to km/h and updating the current position for the next frame.
### 5. Create a method for visualising the inforamtion in the output videos. Using cv2.rectangle and putText to create a frame for the vehicles and adding text in the video.
### 6. Lastly, method for processing the video. Loads the video, model, tracker and analyse with YOLO to detect vehicles. SORT used to track each detected vehicles and estimating their speed based on the method before. When the vehicles crossed the vehicle line, te counter increase by 1. Finally, each frame is visualised and output to a mp4 files showing the total car counts.

---

# Task 2 - Audio Transcription 
# Transcribing audio to text using Whisper model

# Overview
This project build a solution to transcribe audio to text, especially in Malaysian spoken languages.

---

# Approach

1. **Transcribe**  
   Transcribe the audio to text using Whisper model.
   Whisper - model created by OpenAI, converting spoken audio into written text.

2. **Saving File**
   Saving the transcribed text file into txt files.

---
   
## Technologies and Tools Used

| Tool / Library | Purpose |
|-----------------|----------|
| **Python 3** | Main programming language |
| **Whisper** | Model used to transcribe audio to text|
| **Google Colab** | Environment for execution |
| **ChatGPT** | AI tools to improve my works, debugging and understanding some logic such as whisper model |
| **Youtube** | Researching |

---

## Steps to Reproduce

### 1. Downloading and import the packages such as Whisper for audio transcribing.
### 2. Load the **large** whisper model to transcribe the audio especially Malaysian spoken language to improve the accuracy.
### 3. Finally, outputting the transcribed text into txt files after using the whisper model to transcribe.

---
