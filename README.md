Accuracy Comparison Table:-


Config  Epochs  Layers  Neurons  Activation  Optimizer  Test Accuracy(%)
1)     20       1      256        tanh        SGD        85.73%
2)     5        1      128        relu        Adam       95.15%
3)     10       2       64        tanh        Adam       96.81%
4)     20       1       64        relu        SGD        85.06%
5)     10       2       256       tanh        SGD        83.50%
6)     10       2       128       relu        Adam       98.16%
7)     20       2        64       tanh         SGD       84.56%
8)     5        1       128       tanh        Adam       94.32%
9)     10       2       256       relu        Adam       99.16%



Model Summary of the Best-Performing Model:-

Model: "sequential_8"
┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━┓
┃ Layer (type)                    ┃ Output Shape           ┃       Param # ┃
┡━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━┩
│ dense_20 (Dense)                │ (None, 256)            │       200,960 │
├─────────────────────────────────┼────────────────────────┼───────────────┤
│ dense_21 (Dense)                │ (None, 256)            │        65,792 │
├─────────────────────────────────┼────────────────────────┼───────────────┤
│ dense_22 (Dense)                │ (None, 10)             │         2,570 │
└─────────────────────────────────┴────────────────────────┴───────────────┘
 Total params: 269,322 (1.03 MB)
 Trainable params: 269,322 (1.03 MB)
 Non-trainable params: 0 (0.00 B)

