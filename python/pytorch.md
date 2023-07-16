# [Home](../README.md)

### Manage GPUs
```py
os.environ["CUDA_VISIBLE_DEVICES"] = "0"

device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
```

### Create Module
```py
import torch.nn as nn
import torch.nn.functional as F

class Model(nn.Module):
    def __init__(self):
        super().__init__()
        self.conv1 = nn.Conv2d(1, 20, 5)
        self.conv2 = nn.Conv2d(20, 20, 5)

    def forward(self, x):
        x = F.relu(self.conv1(x))
        return F.relu(self.conv2(x))
```


### Dataset
```py
from torch.utils.data import Dataset


class SA1BDataset(Dataset):
    def __init__(self, img_dir: Path, cfg):
        self.entries = list(img_dir.iterdir())
        self.data_mapper = DatasetMapper(**DatasetMapper.from_config(cfg, is_train=False))

    def __len__(self):
        return len(self.entries)

    def __getitem__(self, idx):
        return self.data_mapper(dict(file_name=self.entries[idx]))
```

### Dataloader
```py
from torch.utils.data import DataLoader


train_dataloader = DataLoader(dataset, batch_size=16, shuffle=True, num_workers=10)
```
