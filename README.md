# VistaPath-Coding

The initial check-in of the coding is for the question to perform image segmentation with the give images: raw.jpeg and mask.png. raw.jpeg is the image to be applied with the segmentation algorithm while mask.png is used to evaluate the performance of the algorithm.

# How to run it:

1. Download the two image files and VistaPath_Coding.ipynb into the same project folder.
2. Launch Jupiter Notebook with that project folder.
3. Just run the iPython file. In case you have library errors, please install the libraries first.
4. You can also uncomment the execution function below each function definition to run them step by step. And you can also uncomment the lines with "image_show(...)" which will show you the image processing results for each step.


# Result Analysis:

1. The metrics chosen to evaluate the performanc are: Recall, Precision and F1 Score.
2. The reason to choose them is: Recall measures the ratio of how many are correctly classified as positive out of actual positives. Precision measures the ratio of how many are correctly classified as positive out of all classified positives. In this application, the segmentation area is only a very small amount of the total area of the image. So Accuracy can reach 99% easily and it can't evaluate the performance of the result. However, Recall and Precision can do a better job in this case. And when you change the threshold, the two metrics change in the opposite direction. F1 Score basically is the Harmonic Mean of Precision and Recall and trades off the two. So a good agorithm with good parameters must trade off between them. In this question.

# Further improvement:

1. In this question, my algorithm choose two retangulars for the two areas for tissues. This is only for this specific image. Some object detection DL technoliges can be applied to it so that the algorithm can detect the regions of interest automatically.
2. Some existing segmentation ML/DL algorithms can be used with further research.
