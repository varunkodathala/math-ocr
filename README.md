# math-ocr
It extracts the mathematical equation from input image and converts it into latex format using Convolutional Neural Networks 

# Data
https://www.kaggle.com/xainano/handwrittenmathsymbols

# Architecture for CONVNET - 1
Partial - VGG-16 
1. CONVOLUTION of size (3x3) - 32 filters  --- * 2 (times) + MaxPooling of size (2x2) --- 1 (time)
2. CONVOLUTION of size (3x3) - 64 filters  --- * 2 (times) + MaxPooling of size (2x2) --- 1 (time)
3. CONVOLUTION of size (3x3) - 128 filters  --- * 2 (times) + MaxPooling of size (2x2) --- 1 (time)
4. Flatten - 64 Units --- * 2(times)
5. Softmax Unit -- 82 units

# Procedure that I followed 
 ***( Suggestions Required for any mistakes )***

1. Trained the CNN model based on the architecture - 1 for the data to distinguish the different math symbols 
2. Object Localization is tested using Slinding Window Method for test Image to gain the inference 
3. For classification of localized object (in this case math symbol/number) is either a symbol or blank (probably a background), I trained another model using logistic regression that seperate the objects (symbol/number) with other objects
4. Combined the methods 3 & 4 to recreate the original model


