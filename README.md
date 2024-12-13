# 2024_EE541_G5_project
EE541 Group5 project
Yuanhao Liang and Yuhui Wu

Purpose: This work aims to develop deep learning models for recognizing American Sign Language (ASL) gestures. ASL plays a critical role in facilitating communication for individuals relying on non-verbal interaction and in environments where verbal communication is impractical. However, existing ASL recognition models face challenges in achieving accuracy, real-time performance, and robustness against background noise. Our goal is to construct models that perform well on clean datasets, such as Kaggle-ASL Alphabet, while maintaining strong generalization on noisy datasets like MS-ASL.

Methods: We implemented a multi-layer Convolutional Neural Network (CNN) for gesture recognition on the MNIST-ASL and Kaggle-ASL datasets. To handle video-based ASL recognition, we combined CNN with a Recurrent Neural Network (RNN) to create a CNN-LSTM model, which was evaluated on the WLASL dataset.

Results: The CNN model achieved a test accuracy of 99.33\% on MNIST-ASL and 92.86\% on Kaggle-ASL, demonstrating strong performance of static image classification. On the WLASL dataset, the CNN-LSTM model trained on 10 classes achieved a test accuracy of 72.73\%, while the model trained on 15 classes outperformed it with a test accuracy of 83.76\%, demonstrating that our approach is capable of performing dynamic classification on video data effectively.

----
Img: you can find all the images describing the performance of our models in forlder img
CNN_ASL_code: you can find the CNN model for static image in folder CNN_ASL_code
Dynamic_ASL: you can find the CNN_LSTM model for video in folder Dynamic_ASL

We did not include the training data in this repo, you must download them personally.

Some of the models are training using Apple silicon GPU, tensorflow = 2.16.2, python 3.11