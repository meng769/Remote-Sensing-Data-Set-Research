# Remote-Sensing-Data-Set-Research
## 目录
- 遥感数据集
  - SynRS3D数据集
  - LEVIR数据集
  - MultiResSAR数据集
  - SARptical数据集
- 非遥感数据集
  - REMD数据集
  - Brown数据集
  - MD-syn数据集 
## 遥感数据集
### SynRS3D数据集

SynRS3D数据集包含69,667张高分辨率光学图像。SynRS3D 数据集的单张图像幅宽为 512×512 像素，对应的地面覆盖范围取决于 GSD。

例如，当 GSD 为 0.09m时，单张图像的覆盖范围约为 46.08m × 46.08m（512×0.09m）。

SynRS3D数据集中的图像 GSD 范围为 0.05m~1m。

SynRS3D 数据集中的图像本身是小图，但通过图像拼接技术可以将它们拼接成更大的图像，以满足特定的应用需求。

场景类型：数据集涵盖六种全球城市风格，包括郊区、城市、山地、沙漠、沿海、农村等多种场景，展示了较强的地理多样性。

地表类型：数据集中包含八种地表覆盖类型，包括裸地、草原、开发空间、道路、树木、水体、农业用地、建筑物。

高度信息：SynRS3D不仅提供地表覆盖类型的标注，还提供精确的高度信息（如树木和建筑物的高度），并生成建筑变化掩码。

SynRS3D 数据集下载链接: https://github.com/JTRNEO/SynRS3D

预览图片: ![image](https://github.com/user-attachments/assets/ea0130e5-7041-4985-be9a-9d03434ea6cd)

参考文献: SynRS3D: A Synthetic Dataset for Global 3D Semantic Understanding from Monocular Remote Sensing Imagery http://arxiv.org/abs/2406.18151

创新点：
- SynRS3D数据集：该研究推出了全球最大的合成遥感3D数据集SynRS3D，涵盖六种城市风格，具有69,667张高分辨率光学图像，并包含八种地表类型、精确的高度信息以及建筑变化掩码。这一数据集解决了高质量标注数据获取难度大的问题，尤其是在欠发达地区。
- RS3DAda算法：提出了一种新颖的多任务无监督域自适应算法RS3DAda，旨在从合成数据到真实场景的转换。这种方法结合了土地覆盖分类和高度估计任务，通过自监督训练框架，提升了在真实世界场景中的表现。
- 多任务域自适应：RS3DAda通过高度伪标签生成和地表覆盖伪标签生成，结合高度一致性和地面信息，减少了合成与真实数据之间的域间隙，并在合成数据的训练模型上达到了与真实数据相当甚至更好的表现。
### LEVIR 数据集
LEVIR数据集由大量 800 × 600 像素和0.2m〜1.0m/pix的高分辨率Google Earth图像和超过22k的图像组成。

LEVIR数据集图像GSD范围为 0.2m〜1.0m/pix 

LEVIR数据集涵盖了人类居住环境的大多数类型地面特征，例如城市，乡村，山区和海洋。数据集中未考虑冰川，沙漠和戈壁等极端陆地环境。

数据集中有3种目标类型：飞机，轮船（包括近海轮船和向海轮船）和油罐。所有图像总共标记了11k个独立边界框，包括4,724架飞机，3,025艘船和3,279个油罐。每个图像的平均目标数量为0.5。

预览图片: 
LEVIR数据集下载链接: http://levir.buaa.edu.cn/Code.htm

参考文献: https://ieeexplore.ieee.org/document/8106808

### MultiResSAR数据集
MultiResSAR是一个大规模、多源、多分辨率、多场景的SAR与光学影像配准数据集。

该数据集包含10,850对光学和SAR图像，覆盖了来自四颗商业卫星的SAR数据，分辨率从0.16m到10m不等。

场景类型包括城市、农村、平原、丘陵、山区和水域。

数据集利用了来自四颗SAR卫星的数据，结合自动配准和人工视觉检查，创建了一个全面的SAR-光学图像配准性能评估平台。该平台不仅为传统算法提供了公平的比较基准，还用于评估基于深度学习的配准网络的泛化能力。

MultiResSAR数据集下载链接: https://github.com/betterlll/Multi-Resolution-SAR-dataset-


### SARptical数据集
光学图像的分辨率为 0.2m，SAR 图像的分辨率为 1m。

图像尺寸：112×112 像素

数据集中的每对图像块的中心像素在三维空间中的位置被精确匹配，精度通常在 几米范围内。

SARptical数据集下载链接: https://github.com/zhu-xlab/SARptical
## 非遥感数据集
### SEMD数据集
SEMD数据集是一个包含、语音眼神和动作的数据集，主要用于研究这三者之间的关系。该数据集通过从 YouTube 下载视频并提取面部关键点来构建。

SEMD数据集下载链接: https://github.com/Eddie-Hwang/Speech-Eye-Motion-Dataset

### Brown数据集
Brown数据集是一个图像匹配的经典集合，包含了Liberty、NotreDame和Yosemite三个地方的图像。数据集通过三维重建获取特征点信息和匹配关系，常用于图像处理和计算机视觉研究。

Brown数据集由 1024 x 1024 位图 (.bmp) 图像组成，每个图像包含一个 16 x 16 图像块阵列。每个补丁都被采样为 64 x 64 灰度，具有规范的比例和方向。

预览图片: ![image](https://github.com/user-attachments/assets/21667115-ec5a-4bb1-9ac4-cbc0ab81578a)

参考文献: https://ieeexplore.ieee.org/document/9850980

### MD-syn数据集
MD-syn数据集是由华中科技大学和武汉大学联合创建的多模态图像匹配数据集。它旨在解决跨模态图像匹配中的数据稀缺问题，通过生成模型从RGB图像扩展而来，包含多种模态（如RGB、红外、深度等）和丰富场景。该数据集包含4.8亿对图像，继承了RGB数据的匹配标签和多样性

数据集的图像分辨率未明确提及，但其源数据来自MegaDepth数据集，该数据集的图像分辨率通常为 1024×768像素。

数据集的幅宽（图像宽度）未明确提及，但基于MegaDepth数据集的图像宽度通常为 1024像素。

MD-syn数据集包含七种模态类型，包括RGB、红外、深度、事件、法线图、草图和绘画。该数据集广泛应用于跨模态图像匹配任务，显著提升了模型的泛化能力和零样本性能。

MD-syn数据集下载链接: https://github.com/LSXI7/MINIMA

参考文献: LSXI7/MINIMA: [CVPR 2025] MINIMA: Modality Invariant Image Matching https://arxiv.org/abs/2412.19412
