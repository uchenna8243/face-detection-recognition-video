# Face Detection & Recognition in Video

Detected and recognised faces in a video interview using MTCNN for face detection and an Inception-ResNet model for face recognition, then served the model through a Flask web app.

## Problem
Identifying who appears in a video, and when, is useful for media indexing and archiving. Doing it by hand is slow, so the task was to automate it end to end.

## Process
1. **Frame extraction:** sampled frames from the interview video.
2. **Face detection:** used MTCNN to locate faces and facial landmarks in each frame and crop the faces.
3. **Face embeddings:** passed the cropped faces through a pre-trained Inception-ResNet model to turn each face into a numerical embedding.
4. **Reference set:** built reference embeddings for the known people in the video.
5. **Recognition:** matched each new face to the closest reference embedding using a distance threshold, and labelled the face on the frame.
6. **Deployment:** wrapped the pipeline in a Flask web app so a user can submit an image and get back the recognised faces.

## Tools
Python · PyTorch · facenet-pytorch (MTCNN, Inception-ResNet) · OpenCV · Flask · Jupyter

## Skills shown
Face detection · Embeddings and similarity · Model serving with Flask · End-to-end ML pipeline

## Repository status
The project notebooks and scripts are being prepared for upload and will be added here shortly.

## Programme
Completed as part of the **WorldQuant University Applied AI Lab: Deep Learning for Computer Vision** (Jul 2025).

## Author
**Uchenna Francis Onyeka** · MSc FinTech with Business Analytics, University of Westminster
[LinkedIn](https://www.linkedin.com/in/uchenna-onyeka) · [GitHub](https://github.com/uchenna8243)
