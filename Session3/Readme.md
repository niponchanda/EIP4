Given:  Parameters: 1,172,410, Accuracy on test data is: 82.04
***************************************************************
41st Epoch, parameters: 74,197
Accuracy: 0.8326
***************************************************************
Model definitions

# Define the model
model = Sequential()
model.add(SeparableConv2D(48, 3, 3, border_mode='same', input_shape=(32, 32, 3)))
model.add(Activation('relu'))
model.add(BatchNormalization())
model.add(SeparableConv2D(96, 3, 3))#30 RF 3
model.add(Activation('relu'))
model.add(BatchNormalization())
model.add(SeparableConv2D(96, 3, 3))#28 RF 5
model.add(Activation('relu'))
model.add(BatchNormalization())
model.add(MaxPooling2D(pool_size=(2, 2)))#14 RF 10
model.add(BatchNormalization())
model.add(Dropout(0.2))
model.add(SeparableConv2D(96, 3, 3, border_mode='same'))
model.add(Activation('relu'))
model.add(BatchNormalization())
model.add(SeparableConv2D(96, 3, 3))#12 RF 12
model.add(Activation('relu'))
model.add(BatchNormalization())
model.add(MaxPooling2D(pool_size=(2, 2)))#6 RF 24
model.add(BatchNormalization())
model.add(Dropout(0.2))
model.add(SeparableConv2D(96, 3, 3))#4 RF 26
model.add(Activation('relu'))
model.add(BatchNormalization())
model.add(SeparableConv2D(192, 3, 3, border_mode='same'))
model.add(Activation('relu'))
model.add(BatchNormalization())
model.add(Dropout(0.2))
model.add(SeparableConv2D(num_classes, 4, 4))
model.add(Flatten())
model.add(Activation('softmax'))
******************************************************************************
50 epoch logs:

Epoch 1/50
390/390 [==============================] - 26s 68ms/step - loss: 1.3148 - acc: 0.5271 - val_loss: 1.0046 - val_acc: 0.6437
Epoch 2/50
390/390 [==============================] - 23s 59ms/step - loss: 0.9076 - acc: 0.6776 - val_loss: 0.8965 - val_acc: 0.6850
Epoch 3/50
390/390 [==============================] - 23s 60ms/step - loss: 0.7801 - acc: 0.7217 - val_loss: 0.7706 - val_acc: 0.7281
Epoch 4/50
390/390 [==============================] - 23s 60ms/step - loss: 0.6979 - acc: 0.7537 - val_loss: 0.7042 - val_acc: 0.7536
Epoch 5/50
390/390 [==============================] - 23s 60ms/step - loss: 0.6433 - acc: 0.7755 - val_loss: 0.6809 - val_acc: 0.7661
Epoch 6/50
390/390 [==============================] - 23s 59ms/step - loss: 0.5985 - acc: 0.7892 - val_loss: 0.7417 - val_acc: 0.7512
Epoch 7/50
390/390 [==============================] - 23s 59ms/step - loss: 0.5636 - acc: 0.8021 - val_loss: 0.6382 - val_acc: 0.7865
Epoch 8/50
390/390 [==============================] - 23s 59ms/step - loss: 0.5339 - acc: 0.8129 - val_loss: 0.5941 - val_acc: 0.7998
Epoch 9/50
390/390 [==============================] - 23s 60ms/step - loss: 0.5058 - acc: 0.8210 - val_loss: 0.6038 - val_acc: 0.7940
Epoch 10/50
390/390 [==============================] - 23s 60ms/step - loss: 0.4865 - acc: 0.8295 - val_loss: 0.6015 - val_acc: 0.7964
Epoch 11/50
390/390 [==============================] - 23s 60ms/step - loss: 0.4637 - acc: 0.8368 - val_loss: 0.5798 - val_acc: 0.8023
Epoch 12/50
390/390 [==============================] - 23s 60ms/step - loss: 0.4499 - acc: 0.8426 - val_loss: 0.6058 - val_acc: 0.8013
Epoch 13/50
390/390 [==============================] - 23s 59ms/step - loss: 0.4287 - acc: 0.8492 - val_loss: 0.5762 - val_acc: 0.8096
Epoch 14/50
390/390 [==============================] - 23s 59ms/step - loss: 0.4193 - acc: 0.8508 - val_loss: 0.6306 - val_acc: 0.7944
Epoch 15/50
390/390 [==============================] - 23s 59ms/step - loss: 0.4055 - acc: 0.8568 - val_loss: 0.6198 - val_acc: 0.8015
Epoch 16/50
390/390 [==============================] - 23s 60ms/step - loss: 0.3921 - acc: 0.8621 - val_loss: 0.5802 - val_acc: 0.8107
Epoch 17/50
390/390 [==============================] - 23s 59ms/step - loss: 0.3776 - acc: 0.8655 - val_loss: 0.5680 - val_acc: 0.8119
Epoch 18/50
390/390 [==============================] - 23s 59ms/step - loss: 0.3739 - acc: 0.8676 - val_loss: 0.5696 - val_acc: 0.8142
Epoch 19/50
390/390 [==============================] - 23s 59ms/step - loss: 0.3536 - acc: 0.8743 - val_loss: 0.5581 - val_acc: 0.8215
Epoch 20/50
390/390 [==============================] - 23s 60ms/step - loss: 0.3484 - acc: 0.8751 - val_loss: 0.5895 - val_acc: 0.8162
Epoch 21/50
390/390 [==============================] - 23s 59ms/step - loss: 0.3416 - acc: 0.8788 - val_loss: 0.6299 - val_acc: 0.8080
Epoch 22/50
390/390 [==============================] - 23s 59ms/step - loss: 0.3326 - acc: 0.8816 - val_loss: 0.6129 - val_acc: 0.8135
Epoch 23/50
390/390 [==============================] - 23s 60ms/step - loss: 0.3218 - acc: 0.8864 - val_loss: 0.5897 - val_acc: 0.8148
Epoch 24/50
390/390 [==============================] - 23s 60ms/step - loss: 0.3190 - acc: 0.8851 - val_loss: 0.5829 - val_acc: 0.8209
Epoch 25/50
390/390 [==============================] - 23s 59ms/step - loss: 0.3117 - acc: 0.8894 - val_loss: 0.5991 - val_acc: 0.8179
Epoch 26/50
390/390 [==============================] - 23s 59ms/step - loss: 0.3044 - acc: 0.8916 - val_loss: 0.5863 - val_acc: 0.8169
Epoch 27/50
390/390 [==============================] - 23s 60ms/step - loss: 0.2944 - acc: 0.8938 - val_loss: 0.6104 - val_acc: 0.8142
Epoch 28/50
390/390 [==============================] - 23s 60ms/step - loss: 0.2921 - acc: 0.8954 - val_loss: 0.5877 - val_acc: 0.8255
Epoch 29/50
390/390 [==============================] - 23s 60ms/step - loss: 0.2842 - acc: 0.8961 - val_loss: 0.6268 - val_acc: 0.8183
Epoch 30/50
390/390 [==============================] - 23s 60ms/step - loss: 0.2830 - acc: 0.8986 - val_loss: 0.5803 - val_acc: 0.8255
Epoch 31/50
390/390 [==============================] - 23s 59ms/step - loss: 0.2761 - acc: 0.8993 - val_loss: 0.5556 - val_acc: 0.8297
Epoch 32/50
390/390 [==============================] - 23s 60ms/step - loss: 0.2773 - acc: 0.9002 - val_loss: 0.5972 - val_acc: 0.8243
Epoch 33/50
390/390 [==============================] - 23s 59ms/step - loss: 0.2694 - acc: 0.9018 - val_loss: 0.5933 - val_acc: 0.8283
Epoch 34/50
390/390 [==============================] - 23s 60ms/step - loss: 0.2636 - acc: 0.9041 - val_loss: 0.5840 - val_acc: 0.8251
Epoch 35/50
390/390 [==============================] - 23s 59ms/step - loss: 0.2576 - acc: 0.9077 - val_loss: 0.5848 - val_acc: 0.8267
Epoch 36/50
390/390 [==============================] - 23s 60ms/step - loss: 0.2572 - acc: 0.9065 - val_loss: 0.6274 - val_acc: 0.8237
Epoch 37/50
390/390 [==============================] - 23s 60ms/step - loss: 0.2543 - acc: 0.9071 - val_loss: 0.5775 - val_acc: 0.8288
Epoch 38/50
390/390 [==============================] - 23s 59ms/step - loss: 0.2504 - acc: 0.9072 - val_loss: 0.5819 - val_acc: 0.8299
Epoch 39/50
390/390 [==============================] - 23s 60ms/step - loss: 0.2453 - acc: 0.9111 - val_loss: 0.6464 - val_acc: 0.8183
Epoch 40/50
390/390 [==============================] - 23s 60ms/step - loss: 0.2410 - acc: 0.9123 - val_loss: 0.5851 - val_acc: 0.8314
Epoch 41/50
390/390 [==============================] - 23s 59ms/step - loss: 0.2379 - acc: 0.9135 - val_loss: 0.6040 - val_acc: 0.8326
Epoch 42/50
390/390 [==============================] - 23s 60ms/step - loss: 0.2360 - acc: 0.9141 - val_loss: 0.6030 - val_acc: 0.8306
Epoch 43/50
390/390 [==============================] - 23s 60ms/step - loss: 0.2356 - acc: 0.9134 - val_loss: 0.6309 - val_acc: 0.8237
Epoch 44/50
390/390 [==============================] - 23s 59ms/step - loss: 0.2346 - acc: 0.9152 - val_loss: 0.6266 - val_acc: 0.8226
Epoch 45/50
390/390 [==============================] - 23s 59ms/step - loss: 0.2217 - acc: 0.9194 - val_loss: 0.6441 - val_acc: 0.8273
Epoch 46/50
390/390 [==============================] - 23s 59ms/step - loss: 0.2229 - acc: 0.9199 - val_loss: 0.5979 - val_acc: 0.8324
Epoch 47/50
390/390 [==============================] - 23s 60ms/step - loss: 0.2237 - acc: 0.9189 - val_loss: 0.6398 - val_acc: 0.8259
Epoch 48/50
390/390 [==============================] - 23s 59ms/step - loss: 0.2228 - acc: 0.9199 - val_loss: 0.6130 - val_acc: 0.8316
Epoch 49/50
390/390 [==============================] - 23s 59ms/step - loss: 0.2153 - acc: 0.9219 - val_loss: 0.6514 - val_acc: 0.8213
Epoch 50/50
390/390 [==============================] - 23s 59ms/step - loss: 0.2170 - acc: 0.9207 - val_loss: 0.6052 - val_acc: 0.8295
Model took 1164.76 seconds to train

Accuracy on test data is: 82.95
