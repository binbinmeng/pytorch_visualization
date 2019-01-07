# pytorch_visualization
A tool integrated with some functions to visualize some data and states when training in pytorch.
```
Usage:
root$:/workspace/pytorch_visualization# python visualize.py
AlexNet (
  (features): Sequential (
    (0): Conv2d(3, 64, kernel_size=(11, 11), stride=(4, 4), padding=(2, 2)), weights=((64, 3, 11, 11), (64,)), parameters=23296
    (1): ReLU(inplace), weights=(), parameters=0
    (2): MaxPool2d(kernel_size=3, stride=2, padding=0, dilation=1, ceil_mode=False), weights=(), parameters=0
    (3): Conv2d(64, 192, kernel_size=(5, 5), stride=(1, 1), padding=(2, 2)), weights=((192, 64, 5, 5), (192,)), parameters=307392
    (4): ReLU(inplace), weights=(), parameters=0
    (5): MaxPool2d(kernel_size=3, stride=2, padding=0, dilation=1, ceil_mode=False), weights=(), parameters=0
    (6): Conv2d(192, 384, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1)), weights=((384, 192, 3, 3), (384,)), parameters=663936
    (7): ReLU(inplace), weights=(), parameters=0
    (8): Conv2d(384, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1)), weights=((256, 384, 3, 3), (256,)), parameters=884992
    (9): ReLU(inplace), weights=(), parameters=0
    (10): Conv2d(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1)), weights=((256, 256, 3, 3), (256,)), parameters=590080
    (11): ReLU(inplace), weights=(), parameters=0
    (12): MaxPool2d(kernel_size=3, stride=2, padding=0, dilation=1, ceil_mode=False), weights=(), parameters=0
  ), weights=((64, 3, 11, 11), (64,), (192, 64, 5, 5), (192,), (384, 192, 3, 3), (384,), (256, 384, 3, 3), (256,), (256, 256, 3, 3), (256,)), parameters=2469696
  (classifier): Sequential (
    (0): Dropout(p=0.5), weights=(), parameters=0
    (1): Linear(in_features=9216, out_features=4096, bias=True), weights=((4096, 9216), (4096,)), parameters=37752832
    (2): ReLU(inplace), weights=(), parameters=0
    (3): Dropout(p=0.5), weights=(), parameters=0
    (4): Linear(in_features=4096, out_features=4096, bias=True), weights=((4096, 4096), (4096,)), parameters=16781312
    (5): ReLU(inplace), weights=(), parameters=0
    (6): Linear(in_features=4096, out_features=1000, bias=True), weights=((1000, 4096), (1000,)), parameters=4097000
  ), weights=((4096, 9216), (4096,), (4096, 4096), (4096,), (1000, 4096), (1000,)), parameters=58631144
)
            name class_name        input_shape       output_shape         nb_params
1     features.0     Conv2d  (-1, 3, 224, 224)   (-1, 64, 55, 55)     tensor(23296)
2     features.1       ReLU   (-1, 64, 55, 55)   (-1, 64, 55, 55)                 0
3     features.2  MaxPool2d   (-1, 64, 55, 55)   (-1, 64, 27, 27)                 0
4     features.3     Conv2d   (-1, 64, 27, 27)  (-1, 192, 27, 27)    tensor(307392)
5     features.4       ReLU  (-1, 192, 27, 27)  (-1, 192, 27, 27)                 0
6     features.5  MaxPool2d  (-1, 192, 27, 27)  (-1, 192, 13, 13)                 0
7     features.6     Conv2d  (-1, 192, 13, 13)  (-1, 384, 13, 13)    tensor(663936)
8     features.7       ReLU  (-1, 384, 13, 13)  (-1, 384, 13, 13)                 0
9     features.8     Conv2d  (-1, 384, 13, 13)  (-1, 256, 13, 13)    tensor(884992)
10    features.9       ReLU  (-1, 256, 13, 13)  (-1, 256, 13, 13)                 0
11   features.10     Conv2d  (-1, 256, 13, 13)  (-1, 256, 13, 13)    tensor(590080)
12   features.11       ReLU  (-1, 256, 13, 13)  (-1, 256, 13, 13)                 0
13   features.12  MaxPool2d  (-1, 256, 13, 13)    (-1, 256, 6, 6)                 0
14  classifier.0    Dropout         (-1, 9216)         (-1, 9216)                 0
15  classifier.1     Linear         (-1, 9216)         (-1, 4096)  tensor(37752832)
16  classifier.2       ReLU         (-1, 4096)         (-1, 4096)                 0
17  classifier.3    Dropout         (-1, 4096)         (-1, 4096)                 0
18  classifier.4     Linear         (-1, 4096)         (-1, 4096)  tensor(16781312)
19  classifier.5       ReLU         (-1, 4096)         (-1, 4096)                 0
20  classifier.6     Linear         (-1, 4096)         (-1, 1000)   tensor(4097000)
```
