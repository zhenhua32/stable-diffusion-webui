[TOC]

课程仓库是 https://github.com/huggingface/diffusion-models-class/tree/main


# 下载模型

```python
from huggingface_hub import snapshot_download
import os
os.environ["HF_ENDPOINT"] = "https://hf-mirror.com"

snapshot_download(repo_id="google/ddpm-celebahq-256", local_dir="./model", local_dir_use_symlinks=False)
```

下载数据集

```python
import os
os.environ["HF_ENDPOINT"] = "https://hf-mirror.com"

dataset_name = "huggan/smithsonian_butterflies_subset"
dataset = load_dataset(dataset_name, split="train", cache_dir="./data/smithsonian_butterflies_subset")
```

