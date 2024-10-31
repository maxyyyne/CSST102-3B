# MACHINE PROBLEM 1

## Exploring the Role of Computer Vision and Image Processing in AI

**Name: Maxyne Nuela Ignacio**
**Year & Section: BSCS-4B**
---

### Visual Presentation:

[Uploading 05-MP1-PPTSlideshow-Ignacio4B.mp4…](https://github.com/user-attachments/assets/0992377c-e8b4-4329-add0-b836caf25853)

# Research and Comprehend

## Introduction to Computer Vision
**Start by researching the basic concepts of Computer Vision, focusing on how AI systems process visual information.**

- Computer vision, a field of AI, enables machines to interpret visual data by analyzing images or videos to recognize patterns and objects for applications like object detection and image segmentation (Computer Vision: Algorithms and Applications, Szeliski, 2022).

- One of the basic concepts of Computer Vision is Image Processing. Image processing prepares visual data, while computer vision interprets it to understand scenes and objects, key for applications like face recognition  (Computer Vision: Algorithms and Applications, Szeliski, 2022).

- Another example is Feature extraction that identifies distinctive parts of an image, like edges or textures, helping machines recognize similar patterns in different images (Object Recognition from Local Scale-Invariant Features, Lowe, 1999).

**Understand the role of image processing in AI, including why AI systems must enhance, manipulate, and analyze images effectively.**

- Image processing prepares visual data, enhancing quality and extracting essential details for analysis, helping AI systems interpret images accurately.

- It enables noise reduction, contrast adjustment, and feature extraction, making images clearer and more informative for AI.

- By manipulating visual data, image processing helps AI recognize patterns and objects reliably, powering applications like facial recognition and medical imaging.

## Overview of Image Processing Techniques
**Explore the key techniques used in image processing, such as filtering, edge detection, and segmentation.**

- Image filtering, such as Gaussian or median filters, smooths images and reduces noise, enhancing the quality of visual data for further analysis (Digital Image Processing Techniques for High-Resolution Satellite Imagery, Kaur & Saini, 2021).

- Edge Detection Techniques like the Canny edge detector identify significant transitions in pixel intensity, allowing AI to delineate object boundaries effectively (Real-time Edge Detection with Deep Learning*, Ahmed et al., 2020).

- Image segmentation divides an image into meaningful regions or objects, enabling precise analysis and recognition, crucial for applications like medical imaging and autonomous driving (A Survey of Deep Learning Techniques for Image Segmentation, Akin et al., 2022).

**Identify at least three core techniques and investigate how these techniques help AI systems to extract meaningful information from images.**

- Filtering techniques, such as Gaussian and median filters, are used to reduce noise and enhance image quality. By smoothing images, these filters help AI systems focus on significant features, improving the accuracy of analyzation like object recognition and classification.

- Edge detection algorithms, like the Canny edge detector, identify boundaries within images. This technique allows AI systems to delineate object contours, enabling more effective identification and localization of objects within a scene, which is critical for applications such as autonomous driving and facial recognition.

- Image segmentation techniques partition an image into distinct regions or objects based on characteristics such as color, intensity, or texture. 

# Case Study Selection

**Choose a real-world AI application that utilizes computer vision (e.g., facial recognition systems, autonomous vehicles, or medical imaging).**

My chosen AI application is facial recognition, a technology that "identifies or verifies individuals by analyzing and matching unique facial features in digital images or videos" (Nguyen et al., Journal of Computer Vision Research, 2020).

**Investigate how image processing is used within this application. Focus on the specific techniques applied and their effectiveness in solving visual problems.**

In facial recognition, image processing plays a fundamental role by enabling precise analysis of facial features, which is crucial for accurate identification and verification. Specific techniques such as face detection, feature extraction, face alignment, and image enhancement are widely used, each contributing to the system's overall effectiveness.

- Face detection locates faces within images, often using deep learning models like Multi-task Cascaded Convolutional Networks (MTCNN), which enhance accuracy under different lighting and angles (Zhang et al., 2019).

- Feature extraction quantifies unique facial characteristics, with models like FaceNet using deep learning to capture facial details that improve identification precision (Kumar & Gupta, 2021).

- Face alignment uses geometric transformations to standardize face positions, reducing errors from pose variations and improving recognition accuracy (Liu et al., 2020).

- Image Enhancement Techniques like histogram equalization improve facial feature clarity by normalizing lighting, which enhances detection reliability under various conditions (Chen & Lee, 2019).


# Implementation Creation

**Select a simple problem related to your chosen AI application.**

- A simple problem in facial recognition is accurate detection under poor lighting conditions. Variations in lighting can struggle facial features, leading to missed detections or incorrect matches.

# PROBLEM: inaccurate detection under poor lighting conditions.

**CODE & RESULT: Install Environment**

![Screenshot 2024-10-27 205126](https://github.com/user-attachments/assets/81053895-1131-45ae-88eb-5c6a2bc302d1)

- The command pip install opencv-python installs OpenCV, a powerful library for computer vision tasks, in your Python environment.
- OpenCV provides tools for processing images and videos, enabling tasks such as face detection, image filtering, and object recognition.
- By running this command, users can easily integrate OpenCV into their projects, facilitating advanced visual analysis and manipulation.
- OpenCV supports various platforms and is highly optimized for performance, making it a popular choice among developers and researchers in the field of computer vision.

**CODE & RESULT: Import Libraries**

![Screenshot 2024-10-27 205625](https://github.com/user-attachments/assets/8499410f-5ab9-460c-a8b2-33ee19e4ca67)

- These libraries such as OpenCV for image processing, NumPy for efficient numerical operations, and PIL for enhancing brightness and contrast are essential for improving facial recognition accuracy in challenging lighting conditions.

**CODE & RESULT: Load the Image**

![Screenshot 2024-10-27 210244](https://github.com/user-attachments/assets/1a4a3cc7-5dbe-4002-a17a-5787656667fc)

- This loads and displays the original image, allowing us to visually assess lighting conditions and identify areas where enhancements may be needed to improve facial recognition accuracy.

**CODE & RESULT: Grayscale Conversion**

![Screenshot 2024-10-27 210617](https://github.com/user-attachments/assets/3a6db8f2-5d3d-4371-98d6-9194e27aa298)

- Grayscale conversion simplifies the image, focusing on essential facial features without color distractions.
- It enhances contrast, making facial structures more visible for accurate recognition.
- This reduction in data also speeds up processing, allowing for quicker and more efficient detection in low-light scenarios.

**CODE & RESULT: Gaussian Blur**

![Screenshot 2024-10-27 211052](https://github.com/user-attachments/assets/eaec8c03-4384-4cc3-b5b4-3c3c812f46fd)

- Applying Gaussian blur reduces noise in the image, which can interfere with the detection of facial features.
- This smoothing effect enhances the performance of edge detection algorithms by providing a cleaner image to analyze.
- Blurring also helps to minimize minor details, allowing the model to focus on prominent facial contours for better recognition accuracy.

**CODE & RESULT: Edge Detection**

![Screenshot 2024-10-27 212143](https://github.com/user-attachments/assets/719f13f7-b89b-4a0b-89d1-8e943761ebb3)

- Canny edge detection highlights the prominent edges of facial features, making it easier to identify and extract important structures.
- This technique effectively reduces background noise and distractions, allowing the facial recognition system to focus on relevant contours.
- By emphasizing edges, it improves the overall accuracy of feature extraction, particularly in challenging lighting conditions.

**CODE & RESULT: Histogram Equalization**

![Screenshot 2024-10-27 215320](https://github.com/user-attachments/assets/22ec4008-0a7b-4ef1-8823-0de6ed242b0b)

- Converting the image to grayscale focuses on the essential facial features without color, simplifying the processing.  
- Histogram equalization adjusts image contrast, making facial features more distinguishable, especially in poorly lit areas.  
- This technique enhances visibility of key details, improving recognition accuracy under varying lighting conditions.

**CODE & RESULT: Illumination-Invariant Color Space (HSV) - Brighten and Darken**

![Screenshot 2024-10-27 215518](https://github.com/user-attachments/assets/8a7ed5d4-a2d2-4364-bb4e-90f3169ca38d)

![Screenshot 2024-10-27 215541](https://github.com/user-attachments/assets/e61a2e5a-2f14-4921-934d-3b9b8ff89a16)

- Converting to the HSV color space allows adjustment of only the brightness (V) channel, making it possible to equalize lighting without altering color details.
- By equalizing the V channel, this technique improves the visibility of facial features and makes detection more reliable under varying lighting conditions.
- Brightening the image with the PIL enhancer further enhances visibility, reducing the impact of shadows or low-light areas on facial recognition accuracy.
- Darkening the image helps test the model’s robustness by simulating low-light conditions that challenge facial recognition accuracy.
- By observing performance on a darkened image, adjustments can be made to improve feature detection in real-world low-light scenarios.
- This technique ensures that the model can reliably detect facial features even when lighting conditions are poor or inconsistent.

**CODE & RESULT: Face Detection with HAAR Cascade**

![Screenshot 2024-10-27 215637](https://github.com/user-attachments/assets/79bf3d67-a598-41be-a0d2-68da27fb765b)
![Screenshot 2024-10-27 220136](https://github.com/user-attachments/assets/60b1958e-7090-4d64-abee-31eec062dc21)

- The pre-trained Haar Cascade model for face detection locates faces in the image, ensuring efficiency and accuracy in finding facial regions.  
- Applying face detection on the histogram-equalized image improves feature visibility and accuracy, especially in poor lighting conditions, by enhancing contrast.  
Drawing rectangles around detected faces visually confirms detection success, making it easier to evaluate the model's accuracy in identifying faces within the image.

# CONCLUSION

![6](https://github.com/user-attachments/assets/8d8052ab-304c-46f8-973d-35d6989c368d)

# Extension Activity:

**Research an Emerging Form of Image Processing:**

- Investigate a newer or emerging technique in image processing, such as deep learning- based image analysis.
- Prepare a brief report or additional slide discussing its potential impact on future AI systems.

![7](https://github.com/user-attachments/assets/5835aa3c-6e29-4b15-8d5e-a4f37f43cd9f)


