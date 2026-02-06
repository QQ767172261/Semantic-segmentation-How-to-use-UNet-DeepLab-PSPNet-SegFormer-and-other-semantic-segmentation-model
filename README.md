## 数据集文字描述：
带钢缺陷 钢材表面缺陷分割数据集  
12种缺陷分割


数据集说明：
包含12种缺陷和对应的像素级标签
每种50张
分辨率200x200
位深24
其他信息如下面几张图


12种缺陷为：
abrasionmask,
iron-sheet ash,
liquid,
oxide-scale,
oil-spot,
water-spot,
patch,
punching,
red-iron sheet,
roll-printing,
scratch,
inclusion







带钢表面缺陷分割数据集，每类50张。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/9dd07eb99bd54db2a5a4a54d624cb6ed.png)
1
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/0e8fca723c9d4042a4e0f8867a5b7719.png)
1
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/00c492afe057419b92f906d188f8a620.png)


### ✅ 带钢表面缺陷分割数据集（12类像素级标注）

| **项目** | **详情** |
| :--- | :--- |
| **数据集名称** | 带钢表面缺陷分割数据集 |
| **任务类型** | 图像语义分割（像素级分类） |
| **缺陷类别数** | 12 类 |
| **每类样本数** | 50 张图像 + 对应标签 |
| **总图像数量** | 12 × 50 = 600 张（原始图像）<br>标签图像：600 张（PNG格式，单通道） |
| **图像分辨率** | 200 × 200 像素 |
| **位深** | 24 位（RGB，8位/通道） |
| **图像格式** | `.png` 或 `.jpg`（建议统一为 PNG 以保留质量） |
| **标签格式** | 单通道 PNG 图像，像素值代表类别 ID（0–11） |
| **标注类型** | 像素级语义分割掩膜（Semantic Segmentation Mask） |
| **颜色模式** | RGB 彩色图像（适用于工业相机采集） |
| **适用场景** | 钢材生产质检、自动化缺陷检测、智能制造、工业AI视觉 |

---

### 📋 缺陷类别列表（中英文对照）

| **类别编号** | **英文名称** | **中文解释** |
|-------------|------------------|----------------|
| 0 | `abrasionmask` | 磨损/刮花区域 |
| 1 | `iron-sheet ash` | 铁皮灰烬（氧化残留） |
| 2 | `liquid` | 液体残留（如冷却液） |
| 3 | `oxide-scale` | 氧化皮（高温氧化层脱落） |
| 4 | `oil-spot` | 油斑 |
| 5 | `water-spot` | 水渍 |
| 6 | `patch` | 补丁状异物或修复痕迹 |
| 7 | `punching` | 冲压痕迹/孔洞 |
| 8 | `red-iron sheet` | 红铁皮（未完全去除的锈层） |
| 9 | `roll-printing` | 轧辊压印（来自轧辊表面的重复图案） |
| 10 | `scratch` | 划痕 |
| 11 | `inclusion` | 夹杂物（非金属杂质嵌入表面） |

---![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/75d469384ca54d4490fbf11aab42c563.png)


### 🗂️博主 推荐目录结构

```
steel_defect_segmentation/
├── images/               # 原始带钢表面图像
│   ├── abrasionmask_001.png
│   ├── iron-sheet_ash_001.png
│   └── ...（共600张）
├── masks/                # 像素级标签图像（单通道，0-11值）
│   ├── abrasionmask_001.png
│   ├── iron-sheet_ash_001.png
│   └── ...（共600张）
├── classes.txt           # 类别名称列表（可选）
└── data.yaml             # 配置文件（用于训练框架）
```

---![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/429e928e832143caacdce5d3da870ab8.png)


### 🧪 数据用途与价值

| **应用方向** | **说明** |
|------------|----------|
| **工业质检自动化** | 替代人工巡检，实现高速产线上的实时缺陷识别 |
| **深度学习模型训练** | 可用于 U-Net、DeepLab、PSPNet、SegFormer 等语义分割模型训练 |
| **学术研究与论文** | 提供高质量的小样本多类别工业缺陷数据支持 |
| **竞赛与项目开发** | 适合作为钢铁行业 AI 质检系统的基准数据集 |

---

为了创建一个表格来描述您提供的带钢表面缺陷分割数据集，并附上相应的训练代码，我们需要先明确一些信息。根据您的描述，数据集包含12种不同的缺陷类型，每种缺陷有50张图片及其对应的像素级标签（掩码），所有图像和掩码的分辨率为200x200，位深为24位。

### 数据集结构表

以下是一个简单的表格示例，用于展示数据集中的各类缺陷：

| 序号 | 缺陷名称            | 图片数量 | 分辨率  | 位深 |
|------|-------------------|---------|--------|------|
| 1    | abrasionmask       | 50      | 200x200 | 24   |
| 2    | iron-sheet ash     | 50      | 200x200 | 24   |
| 3    | liquid             | 50      | 200x200 | 24   |
| 4    | oxide-scale        | 50      | 200x200 | 24   |
| 5    | oil-spot           | 50      | 200x200 | 24   |
| 6    | water-spot         | 50      | 200x200 | 24   |
| 7    | patch              | 50      | 200x200 | 24   |
| 8    | punching           | 50      | 200x200 | 24   |
| 9    | red-iron sheet     | 50      | 200x200 | 24   |
| 10   | roll-printing      | 50      | 200x200 | 24   |
| 11   | scratch            | 50      | 200x200 | 24   |
| 12   | inclusion          | 50      | 200x200 | 24   |

### 训练代码示例

下面提供了一个简单的基于PyTorch框架的训练代码示例。此代码旨在演示如何加载数据集、定义模型、损失函数及优化器，并进行训练。

```python
import torch
from torch import nn, optim
from torch.utils.data import DataLoader, Dataset
from torchvision import transforms, models
from sklearn.model_selection import train_test_split

# 假设我们有一个自定义的数据集类MyDataset
class MyDataset(Dataset):
    def __init__(self, image_paths, mask_paths, transform=None):
        self.image_paths = image_paths
        self.mask_paths = mask_paths
        self.transform = transform
        
    def __len__(self):
        return len(self.image_paths)
    
    def __getitem__(self, idx):
        image_path = self.image_paths[idx]
        mask_path = self.mask_paths[idx]
        
        image = Image.open(image_path).convert("RGB")
        mask = Image.open(mask_path).convert("L")  # 灰度图像
        
        if self.transform:
            image = self.transform(image)
            mask = self.transform(mask)
            
        return image, mask

# 定义转换操作
transform = transforms.Compose([
    transforms.Resize((200, 200)),
    transforms.ToTensor(),
])

# 加载并划分数据集
image_paths = ["path/to/your/images"] * 600  # 替换为实际路径列表
mask_paths = ["path/to/your/masks"] * 600  # 替换为实际路径列表
train_images, val_images, train_masks, val_masks = train_test_split(image_paths, mask_paths, test_size=0.2)

train_dataset = MyDataset(train_images, train_masks, transform=transform)
val_dataset = MyDataset(val_images, val_masks, transform=transform)

train_loader = DataLoader(train_dataset, batch_size=16, shuffle=True)
val_loader = DataLoader(val_dataset, batch_size=16, shuffle=False)

# 使用预训练模型作为基础
model = models.segmentation.fcn_resnet50(pretrained=True, num_classes=21)
model.classifier[4] = nn.Conv2d(512, 12, kernel_size=1)  # 修改输出类别数为12

# 损失函数与优化器
criterion = nn.CrossEntropyLoss()
optimizer = optim.Adam(model.parameters(), lr=0.001)

# 训练循环
for epoch in range(epochs):
    model.train()
    for images, masks in train_loader:
        optimizer.zero_grad()
        outputs = model(images)['out']
        loss = criterion(outputs, masks)
        loss.backward()
        optimizer.step()
    print(f"Epoch {epoch+1}, Loss: {loss.item()}")
```

以上文字及代码仅供参考学习使用。
