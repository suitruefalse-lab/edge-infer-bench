backends 中存储推理后端适配层（让“换后端”像换插件）：
torch_eager.py：PyTorch 普通推理
torch_compile.py：PyTorch 2 的 torch.compile 推理（注意 warmup/编译开销）
onnxruntime.py：ONNX Runtime 推理 + graph optimization + profiling 输出
