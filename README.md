# TensorFlowBenchmark

## 特色

- 適應中國大陸網路環境，以已經在 repo 內準備好 dataset，並於程式碼中指定相對路徑，不需要 proxy。
- 在 Apple Silicon 或 Intel/CUDA 平台上(應該)都可以直接使用 GPU。

## 參考數據

- MacBook Air 2018 i5-2CPU 8/256  : 89s/epoch (無法使用 Intel GPU)
- MacBook Air M1 16/512 8CPU/7GPU : 13s/epoch (GPU)
- NVIDIA GA100 [A100 PCIe 40GB]x2 :  3s/epoch (GPU)
