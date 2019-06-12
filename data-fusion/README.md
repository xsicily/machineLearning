# Multimodal Fusion Project
##                  ---Score level fusing of face and voice for identity verification

# Descriptions

  Multi-biometric systems fusion information from multiple biometric sources in order to achieve better recognition performance and to overcome some limitations of uni-biometric systems. Fusion can be performed at four different levels of information, namely, sensor, feature, match score and decision levels. Score level fusion is popular used. The project is aim to do score level fusing of face and voice by different fusion methods for identity verification.

# Data
  4 csv files: each files include 3 columns marked as face, voice and label

-Train_negative (wolf training data): 40000 * 3
-Train_positive (sheep training data): 600 * 3
-Test_negative (wolf testing data): 111800 * 3
-Test_positive (sheep training data): 400 * 3

# Jupyter Notebook

  This notebook shows the framework of this project including requirements, the pre-prepared error calculations and some hints for each task. 

  Task 1: Verification Error from Voice
  Task 2: Verification Error from Face and Voice using a Simple Sum
  Task 3: Weighted Sum Fusion
  Task 4: Implement One Classifier-based Fusion (SVM or Logistic Regression)
  Task 5: One Density-based Score Fusion

# Analysis tools

	Language: Python 3
	Libraries: Numpy, Pandas, sklearn

# Summary

  According to the testing errors from different approach, we can see that fusion reduces the errors compared with uni-modality. Weight sum could be better than simple sum. But the result is opposite. SVM classifier is one good way to do multi-modal fusion. But when biometric score fusion is considered as a classification problem, it may pose some challenges like unbalanced training set. In this project, the number of wolves training data is much more than the number of sheep training data. One density based fusion approach has the advantage that it directly achieves optimal performance at any desired operating point, provided the score densities are estimated accurately.
