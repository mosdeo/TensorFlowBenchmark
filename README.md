# TensorFlowBenchmark

## 特色

- 適應中國大陸網路環境，以已經在 repo 內準備好 dataset，並於程式碼中指定相對路徑，不需要 proxy。
- 在 Apple Silicon 或 Intel/CUDA 平台上(應該)都可以直接使用 GPU。

## 參考數據

- MacBook Air 2018 i5 2CPU 8/256  : 87s/epoch (無法使用 Intel GPU)
- MacBook Air M1 8CPU/7GPU 16/512 : 9.5s/epoch (GPU)
- MacBook Air M2 8CPU/10GPU 24/2T : 8.25s/epoch (GPU)
- NVIDIA GA100 [A100 PCIe 40GB]x2 :  3s/epoch (GPU)
