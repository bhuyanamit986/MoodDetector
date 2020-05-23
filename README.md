# MoodDetector
# Introduction

---

Facial emotion recognition is the process of detecting human emotions from facial expressions. The human brain recognizes emotions automatically, and software has now been developed that can recognize emotions as well. This technology is becoming more accurate all the time, and will eventually be able to read emotions as well as our brains do. 

AI can detect emotions by learning what each facial expression means and applying that knowledge to the new information presented to it. Emotional artificial intelligence, or emotion AI, is a technology that is capable of reading, imitating, interpreting, and responding to human facial expressions and emotions.

---

# Summary of Model

---

```
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
input_1 (InputLayer)         (None, 64, 64, 3)         0         
_________________________________________________________________
zero_padding2d_1 (ZeroPaddin (None, 66, 66, 3)         0         
_________________________________________________________________
conv1 (Conv2D)               (None, 64, 64, 16)        448       
_________________________________________________________________
batch1 (BatchNormalization)  (None, 64, 64, 16)        64        
_________________________________________________________________
activation_1 (Activation)    (None, 64, 64, 16)        0         
_________________________________________________________________
pool1 (MaxPooling2D)         (None, 32, 32, 16)        0         
_________________________________________________________________
zero_padding2d_2 (ZeroPaddin (None, 34, 34, 16)        0         
_________________________________________________________________
conv2 (Conv2D)               (None, 32, 32, 32)        4640      
_________________________________________________________________
batch2 (BatchNormalization)  (None, 32, 32, 32)        128       
_________________________________________________________________
activation_2 (Activation)    (None, 32, 32, 32)        0         
_________________________________________________________________
pool2 (MaxPooling2D)         (None, 16, 16, 32)        0         
_________________________________________________________________
zero_padding2d_3 (ZeroPaddin (None, 18, 18, 32)        0         
_________________________________________________________________
flatten_1 (Flatten)          (None, 10368)             0         
_________________________________________________________________
dropout_1 (Dropout)          (None, 10368)             0         
_________________________________________________________________
fc1 (Dense)                  (None, 10)                103690    
_________________________________________________________________
dropout_2 (Dropout)          (None, 10)                0         
_________________________________________________________________
fc2 (Dense)                  (None, 1)                 11        
=================================================================
Total params: 108,981
Trainable params: 108,885
Non-trainable params: 96
_________________________________________________________________
```

---

# Conclusion

---

- Training Loss      =>     0.0438 
 - Training Accuracy  =>    0.9850  
 - Test Loss          =>    0.093871961832
 - Test Accuracy      =>    0.960000003974
 
 ---
