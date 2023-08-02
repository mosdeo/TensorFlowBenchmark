# TensorFlowBenchmark

## Docker_arm64v8
- for Apple Silicon M1/M2/...
- 目前似乎無法使用 GPU

## Docker_amd64
- for Intel CPU with CUDA GPU
- docker run --gpus all -i verify

## 參考數據

- MacBook Air M2 8CPU/10GPU 24/2T : 80.4s/epoch (GPU)
```
Epoch 1/5
782/782 [==============================] - 82s 100ms/step - loss: 4.5111 - accuracy: 0.0912
Epoch 2/5
782/782 [==============================] - 77s 99ms/step - loss: 4.1982 - accuracy: 0.1110
Epoch 3/5
782/782 [==============================] - 78s 99ms/step - loss: 3.6741 - accuracy: 0.1700
Epoch 4/5
782/782 [==============================] - 82s 105ms/step - loss: 3.4374 - accuracy: 0.2094
Epoch 5/5
782/782 [==============================] - 83s 106ms/step - loss: 3.2929 - accuracy: 0.2468
```

- NVIDIA GA100 [A100 PCIe 40GB]x2 :  47.6s/epoch (Only 1GPU, usage=33%)
```
782/782 [==============================] - 73s 60ms/step - loss: 4.5955 - accuracy: 0.0829
Epoch 2/5
782/782 [==============================] - 40s 51ms/step - loss: 4.0041 - accuracy: 0.1376
Epoch 3/5
782/782 [==============================] - 40s 51ms/step - loss: 3.9703 - accuracy: 0.1533
Epoch 4/5
782/782 [==============================] - 45s 57ms/step - loss: 4.0180 - accuracy: 0.1366
Epoch 5/5
782/782 [==============================] - 40s 52ms/step - loss: 3.6619 - accuracy: 0.1691
```
