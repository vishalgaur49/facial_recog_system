# facial_recognition_system

This code has three notebook which do the following tasks:
1. Face_detection_clustering.ipynb : Takes a folder containing images as input and gives a directory containing all the aligned faces found in the images. Then cluster the faces into k clusters (finds k using two different methods) and give a folder containing folders with similar faces clustered. Caution: clustering is not ideal and you may have to filter this clustered images to create the training data.
Training directory- data
                        ---face1
                                image1
                                image2
                                ...
                        ---face2
                                image1
                                image2

2. Facial_recog_training.ipynb: Takes the training data and encode each face to create Xtrain and create ytrain with category number. Use simple neural network to fit the model and save model (weights/bias) as keras model.
3. face_recog_system.ipynb: Takes webcam feed as input and predict the face category using pre saved model.
