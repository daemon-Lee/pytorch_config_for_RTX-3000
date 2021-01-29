# Pytorch config for RTX-3000

Some versions of pytorch and cuda for the new RTX-3000 series are still unavailable.

To check for compatibility, run:
```bash
  python -c "import torch;print(torch.max(torch.rand((30,30),device='cuda')))"
```

You should try to upgrading Pytorch to 1.7.1 by using
```bash
  pip install torch==1.7.1+cu110 torchvision==0.8.2+cu110 torchaudio===0.7.2 -f https://download.pytorch.org/whl/torch_stable.html
```

If running time is timeout
```bash
  pip install --default-timeout=100 future
```
