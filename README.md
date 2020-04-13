# math-ocr
It extracts the mathematical equation from input image and converts it into latex format using Convolutional Neural Networks 

# Data
https://www.kaggle.com/xainano/handwrittenmathsymbols

# Architecture
Partial - VGG-16 
1. CONVOLUTION of size (3x3) - 32 filters  --- * 2 (times) + MaxPooling of size (2x2) --- 1 (time)
2. CONVOLUTION of size (3x3) - 64 filters  --- * 2 (times) + MaxPooling of size (2x2) --- 1 (time
3. CONVOLUTION of size (3x3) - 128 filters  --- * 2 (times) + MaxPooling of size (2x2) --- 1 (time)
4. Flatten - 64 Units --- * 2(times)
5. Softmax Unit -- 82 units
