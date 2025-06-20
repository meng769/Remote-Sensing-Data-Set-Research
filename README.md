# Remote-Sensing-Data-Set-Research
## 目录
- 遥感数据集
  - MultiResSAR数据集
  - SARptical数据集
  - SEN1-2数据集
  - SARBuD 1.0 数据集
- 非遥感数据集
  - Brown数据集
  - MD-syn数据集 
## 遥感数据集
### MultiResSAR数据集
MultiResSAR是一个大规模、多源、多分辨率、多场景的SAR与光学影像配准数据集。

该数据集包含10,850对光学和SAR图像，覆盖了来自四颗商业卫星的SAR数据，分辨率: 0.16m~10m。

场景类型包括城市、农村、平原、丘陵、山区和水域。

数据集利用了来自四颗SAR卫星的数据，结合自动配准和人工视觉检查，创建了一个全面的SAR-光学图像配准性能评估平台。该平台不仅为传统算法提供了公平的比较基准，还用于评估基于深度学习的配准网络的泛化能力。

预览图片: ![image](https://github.com/user-attachments/assets/be07fa4a-3e06-49f6-8122-efc63efe8112)

MultiResSAR数据集下载链接: https://github.com/betterlll/Multi-Resolution-SAR-dataset-


### SARptical数据集
光学图像的分辨率为 0.2m，SAR 图像的分辨率为 1m。

图像尺寸：112×112 像素

数据集中的每对图像块的中心像素在三维空间中的位置被精确匹配，精度通常在 几米范围内。

预览图片: 

<img width="370" alt="d189a458f33a5fec98a59bb32627528" src="https://github.com/user-attachments/assets/703db1ba-1964-4d98-9279-7b3e76a0d4ca" />
<img width="375" alt="7c2240dd93c2bb4b1658736f562e7f2" src="https://github.com/user-attachments/assets/d954c18b-a866-433e-83fb-6f7638323f84" />

SARptical数据集下载链接: https://github.com/zhu-xlab/SARptical

### SEN1-2数据集
SEN1-2数据集包含了由 Sentinel-1 和 Sentinel-2 卫星分别获取的 282,384 对对应的合成孔径雷达（SAR）和光学图像区域。
这些区域分布在地球的陆地表面，并涵盖了所有四个气象季节。这种数据集结构反映了这一点。

对于 SAR 区域，提供了 8 位单通道图像，其代表的是以分贝为单位的零散射率值。
对于光学区域，使用的是 8 位彩色图像，分别代表第 4、3 和 2 个波段。

SEN1-2数据集由小图组成,但可按照一定的办法拼成大图。

SAR和光学的GSD: 10m/pix

预览图片: 

<img width="850" alt="392be66bab033c4046d890336774b9f" src="https://github.com/user-attachments/assets/5df37b7d-0a48-43ea-9c87-3f0ddeafbbac" />

SEN1-2数据集下载链接: https://dataserv.ub.tum.de/index.php/s/m1436631

### SARBuD 1.0 数据集
SARBuD 1.0（SAR Building Dataset）是一个面向深度学习的中高分辨率 SAR 建筑数据集，由中国科学院空天信息创新研究院基于高分三号（GF-3）卫星的精细模式单极化 SAR 影像构建。

SARBuD 1.0 数据集包含 60,000 张 256×256 像素的有效建筑区样本切片，以及 80,000 张覆盖多种其他地物类型的负样本切片。

SARBuD 1.0 数据集基于 GF-3 卫星的精细模式单极化 SAR 影像，分辨率为 10m。

数据集涵盖中国不同区域的多种地形场景类型和分布类型，包括大面积聚集城区和小范围山区乡镇。

所有建筑区样本均通过高分辨率光学图像手动标注。

预览图片: 

![image](https://github.com/user-attachments/assets/e9625d8e-b8c6-4320-8c41-03bf036c8ea7)

SARBuD 1.0 数据集下载链接: https://github.com/CAESAR-Radi/SARBuD

## 非遥感数据集

### Brown数据集
Brown数据集是一个图像匹配的经典集合，包含了Liberty、NotreDame和Yosemite三个地方的图像。数据集通过三维重建获取特征点信息和匹配关系，常用于图像处理和计算机视觉研究。

Brown数据集由 1024 x 1024 位图 (.bmp) 图像组成，每个图像包含一个 16 x 16 图像块阵列。每个补丁都被采样为 64 x 64 灰度，具有规范的比例和方向。

预览图片: 

![image](https://github.com/user-attachments/assets/21667115-ec5a-4bb1-9ac4-cbc0ab81578a)

参考文献: https://ieeexplore.ieee.org/document/9850980

### MD-syn数据集
MD-syn数据集是由华中科技大学和武汉大学联合创建的多模态图像匹配数据集。它旨在解决跨模态图像匹配中的数据稀缺问题，通过生成模型从RGB图像扩展而来，包含多种模态（如RGB、红外、深度等）和丰富场景。

MD-syn数据集包含七种模态类型，包括RGB、红外、深度、事件、法线图、草图和绘画，广泛应用于跨模态图像匹配任务，显著提升了模型的泛化能力和零样本性能。

该数据集包含4.8亿对图像，继承了RGB数据的匹配标签和多样性。

数据集的图像分辨率未明确提及，但其源数据来自MegaDepth数据集，该数据集的图像分辨率通常为1024×768像素。

数据集的幅宽（图像宽度）未明确提及，但基于MegaDepth数据集的图像宽度通常为1024像素。

预览图片: ![image](https://github.com/user-attachments/assets/e492e996-8f17-4716-8637-a969e4e66de9)

MD-syn数据集下载链接: https://github.com/LSXI7/MINIMA

参考文献: https://arxiv.org/abs/2412.19412
