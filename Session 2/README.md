Assignment for EIP 4 session 2:

NINTH: https://github.com/niponchanda/EIP4/blob/master/Session%202/NINTH.ipynb

13.1k Params
99.43 VAcc (11th Epoch)

Logs of 20 epochs:
****************************************************************
Train on 60000 samples, validate on 10000 samples
Epoch 1/20

Epoch 00001: LearningRateScheduler setting learning rate to 0.003.
60000/60000 [==============================] - 23s 379us/step - loss: 0.1204 - acc: 0.9507 - val_loss: 0.0323 - val_acc: 0.9900
Epoch 2/20

Epoch 00002: LearningRateScheduler setting learning rate to 0.0022744503.
60000/60000 [==============================] - 12s 192us/step - loss: 0.1106 - acc: 0.9521 - val_loss: 0.0375 - val_acc: 0.9883
Epoch 3/20

Epoch 00003: LearningRateScheduler setting learning rate to 0.0018315018.
60000/60000 [==============================] - 11s 190us/step - loss: 0.1025 - acc: 0.9553 - val_loss: 0.0300 - val_acc: 0.9917
Epoch 4/20

Epoch 00004: LearningRateScheduler setting learning rate to 0.0015329586.
60000/60000 [==============================] - 11s 189us/step - loss: 0.1027 - acc: 0.9536 - val_loss: 0.0247 - val_acc: 0.9917
Epoch 5/20

Epoch 00005: LearningRateScheduler setting learning rate to 0.0013181019.
60000/60000 [==============================] - 11s 188us/step - loss: 0.0984 - acc: 0.9558 - val_loss: 0.0223 - val_acc: 0.9928
Epoch 6/20

Epoch 00006: LearningRateScheduler setting learning rate to 0.0011560694.
60000/60000 [==============================] - 11s 189us/step - loss: 0.0931 - acc: 0.9572 - val_loss: 0.0225 - val_acc: 0.9935
Epoch 7/20

Epoch 00007: LearningRateScheduler setting learning rate to 0.0010295127.
60000/60000 [==============================] - 11s 189us/step - loss: 0.0946 - acc: 0.9570 - val_loss: 0.0230 - val_acc: 0.9934
Epoch 8/20

Epoch 00008: LearningRateScheduler setting learning rate to 0.0009279307.
60000/60000 [==============================] - 11s 190us/step - loss: 0.0921 - acc: 0.9564 - val_loss: 0.0245 - val_acc: 0.9924
Epoch 9/20

Epoch 00009: LearningRateScheduler setting learning rate to 0.0008445946.
60000/60000 [==============================] - 11s 189us/step - loss: 0.0916 - acc: 0.9557 - val_loss: 0.0249 - val_acc: 0.9931
Epoch 10/20

Epoch 00010: LearningRateScheduler setting learning rate to 0.0007749935.
60000/60000 [==============================] - 11s 188us/step - loss: 0.0908 - acc: 0.9568 - val_loss: 0.0210 - val_acc: 0.9943
Epoch 11/20

Epoch 00011: LearningRateScheduler setting learning rate to 0.0007159905.
60000/60000 [==============================] - 11s 188us/step - loss: 0.0885 - acc: 0.9572 - val_loss: 0.0220 - val_acc: 0.9940
Epoch 12/20

Epoch 00012: LearningRateScheduler setting learning rate to 0.000665336.
60000/60000 [==============================] - 11s 189us/step - loss: 0.0870 - acc: 0.9586 - val_loss: 0.0231 - val_acc: 0.9929
Epoch 13/20

Epoch 00013: LearningRateScheduler setting learning rate to 0.0006213753.
60000/60000 [==============================] - 11s 188us/step - loss: 0.0869 - acc: 0.9584 - val_loss: 0.0257 - val_acc: 0.9925
Epoch 14/20

Epoch 00014: LearningRateScheduler setting learning rate to 0.0005828638.
60000/60000 [==============================] - 11s 190us/step - loss: 0.0865 - acc: 0.9584 - val_loss: 0.0224 - val_acc: 0.9931
Epoch 15/20

Epoch 00015: LearningRateScheduler setting learning rate to 0.0005488474.
60000/60000 [==============================] - 12s 192us/step - loss: 0.0872 - acc: 0.9565 - val_loss: 0.0199 - val_acc: 0.9940
Epoch 16/20

Epoch 00016: LearningRateScheduler setting learning rate to 0.0005185825.
60000/60000 [==============================] - 11s 188us/step - loss: 0.0827 - acc: 0.9594 - val_loss: 0.0214 - val_acc: 0.9934
Epoch 17/20

Epoch 00017: LearningRateScheduler setting learning rate to 0.000491481.
60000/60000 [==============================] - 11s 188us/step - loss: 0.0831 - acc: 0.9593 - val_loss: 0.0228 - val_acc: 0.9933
Epoch 18/20

Epoch 00018: LearningRateScheduler setting learning rate to 0.0004670715.
60000/60000 [==============================] - 11s 189us/step - loss: 0.0825 - acc: 0.9605 - val_loss: 0.0220 - val_acc: 0.9935
Epoch 19/20

Epoch 00019: LearningRateScheduler setting learning rate to 0.0004449718.
60000/60000 [==============================] - 11s 189us/step - loss: 0.0839 - acc: 0.9596 - val_loss: 0.0215 - val_acc: 0.9942
Epoch 20/20

Epoch 00020: LearningRateScheduler setting learning rate to 0.000424869.
60000/60000 [==============================] - 11s 188us/step - loss: 0.0864 - acc: 0.9563 - val_loss: 0.0211 - val_acc: 0.9940
***********************************************************************

Result of model.evaluate:

[0.021084329184598755, 0.994]

Strategy:

- Started with 16 filter for using less parameter.

- Used 1x1 kernel for merging of features.

- Used maxpooling to reduce the parameter.

-  Layers:

   3x3 kernel ------26x26 RF 3x3
   
   3x3 kernel ------24x24 RF 5x5
   
   1x1 kernel ------24x24 RF 5x5
   
   maxpooling(2x2)--12x12 RF 10x10
   
   3x3 kernel ------10x10 RF 12x12
   
   1x1 kernel ------10x10 RF 12x12
   
   3x3 kernel ------8x8   RF 14x14
   
   1x1 kernel ------8x8   RF 14x14
   
   3x3 kernel ------6x6   RF 16x16
   
   1x1 kernel ------6x6   RF 16x16



 
