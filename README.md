# EVA5-Session4

## Assignment Tasks

99.4% validation accuracy
Less than 20k Parameters
You can use anything from above you want. 
Less than 20 Epochs
No fully connected layer

## My Model

The total number of parameters i achieved are displayed below. I got 99.4% accuracy once.

        ----------------------------------------------------------------
                Layer (type)               Output Shape         Param #
        ================================================================
                    Conv2d-1            [-1, 8, 26, 26]              80
                      ReLU-2            [-1, 8, 26, 26]               0
               BatchNorm2d-3            [-1, 8, 26, 26]              16
                    Conv2d-4           [-1, 16, 24, 24]           1,168
                      ReLU-5           [-1, 16, 24, 24]               0
               BatchNorm2d-6           [-1, 16, 24, 24]              32
                    Conv2d-7            [-1, 8, 24, 24]             136
                 MaxPool2d-8            [-1, 8, 12, 12]               0
                   Dropout-9            [-1, 8, 12, 12]               0
                   Conv2d-10           [-1, 16, 10, 10]           1,168
                     ReLU-11           [-1, 16, 10, 10]               0
              BatchNorm2d-12           [-1, 16, 10, 10]              32
                   Conv2d-13             [-1, 16, 8, 8]           2,320
                     ReLU-14             [-1, 16, 8, 8]               0
              BatchNorm2d-15             [-1, 16, 8, 8]              32
                MaxPool2d-16             [-1, 16, 4, 4]               0
                  Dropout-17             [-1, 16, 4, 4]               0
                   Conv2d-18             [-1, 32, 2, 2]           4,640
                   Conv2d-19             [-1, 10, 2, 2]             330
        ================================================================
        Total params: 9,954
        Trainable params: 9,954
        Non-trainable params: 0


        loss=0.021394284442067146 batch_id=468: 100%|██████████| 469/469 [00:13<00:00, 34.63it/s]
          0%|          | 0/469 [00:00<?, ?it/s]
        Test set: Average loss: 0.0202, Accuracy: 9942/10000 (99.42%)


        loss=0.0219403225928545 batch_id=468: 100%|██████████| 469/469 [00:13<00:00, 34.73it/s]
          0%|          | 0/469 [00:00<?, ?it/s]
        Test set: Average loss: 0.0200, Accuracy: 9937/10000 (99.37%)

        loss=0.008834498934447765 batch_id=468: 100%|██████████| 469/469 [00:13<00:00, 35.03it/s]
        Test set: Average loss: 0.0218, Accuracy: 9926/10000 (99.26%)

