Celebrity Face Matching Project
This project matches a person's face to the most similar celebrity face using the CelebA dataset. It uses deep learning for face detection, embedding generation, and cosine similarity for matching.

Project Steps
Step 1: Dataset Exploration
Used the CelebA dataset which contains celebrity images and attribute files.

Loaded image names and basic information.

Step 2: Face Detection and Alignment
Used MTCNN to detect and crop faces from the original images.

Aligned and saved only the face parts for further use.

Step 3: Generate Face Embeddings
Used FaceNet model via the DeepFace library to generate embeddings.

Stored embeddings in a dictionary with image names as keys.

Step 4: Cosine Similarity Matching
Converted embeddings to a matrix.

Used cosine similarity to find which images are most similar to each other.

Stored the closest match for each face.

Step 5: Matching a New Face
Created a function to match a new face image against the aligned faces.

The function returns the best match and the similarity score.

Step 6: Display Result
Used OpenCV to display the matched celebrity image.

Technologies Used
Python

TensorFlow

DeepFace

MTCNN

NumPy

OpenCV

scikit-learn

How to Use
Place your own image in the project folder.

Call the function match_celebrity("your_image_path.jpg").

The function returns the name of the most similar celebrity and a similarity score.

The matched image can be displayed using OpenCV or matplotlib.

Dataset
CelebA Dataset is used for this project.

It contains over 200,000 celebrity face images.

Download from the official site: http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html
