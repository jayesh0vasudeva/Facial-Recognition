# Facial-Recognition
Hi guys!
i have tried to make this code as self explanatory as possible but there are still afew things that i would like to you about
1. Haar Cascade
   
   You might be wondering what is haar cascade and how does it work ?
   
   I will not go into too much details but the thing is algorithm works on the basis of positive images(images of faces)
   and negative images(images without faces) to help train the classifier and afterwards we extract the features.
   
   You might wonder how do we calculate such features !!??
   
   each feature is a single value that we calculate by subtracting the the sum of pixels under white rectangle from the sum of    pixels under black rectangle.
   
   what it really does is that it creates a rectangular window and which scans a particular area using edge features, line        features and four rectangular features.
   it doesn't go through all the features at the same time rather it creates stages and distribute the features among the          stages as it saves time.If it doesn't find that particular feature than rather than going through different features it        skips the sub-window and move on to the next one.
   
   for further details you can go through the following links:
   https://docs.opencv.org/3.3.0/d7/d8b/tutorial_py_face_detection.html
   https://docs.opencv.org/3.3.0/dc/d88/tutorial_traincascade.html
