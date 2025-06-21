# Remote-Sensing-Data-Set-Research
## 目录
- 遥感数据集
  - MultiResSAR数据集
  - SARptical数据集
  - SEN1-2数据集
  - SARBuD 1.0数据集
  - YeSeg数据集
  - OS-Eval数据集
  - WHY SAR OPT数据集
  - SAR2Opt Heterogeneous数据集
  - QXS-SAROPT数据集数据集
  - University1652-Baseline
  - OS-dataset
  - SOPatch数据集
- 非遥感数据集
  - Brown数据集
  - MD-syn数据集
  - Multimodal Image Matching Datasets
  - 
## 遥感数据集
### MultiResSAR数据集
MultiResSAR是一个大规模、多源、多分辨率、多场景的SAR与光学影像配准数据集。

该数据集包含10,850对光学和SAR图像，覆盖了来自四颗商业卫星的SAR数据，分辨率: 0.16m~10m。

场景类型包括城市、农村、平原、丘陵、山区和水域。

数据集利用了来自四颗SAR卫星的数据，结合自动配准和人工视觉检查，创建了一个全面的SAR-光学图像配准性能评估平台。该平台不仅为传统算法提供了公平的比较基准，还用于评估基于深度学习的配准网络的泛化能力。

示例图片: ![image](https://github.com/user-attachments/assets/be07fa4a-3e06-49f6-8122-efc63efe8112)

MultiResSAR数据集下载链接: https://github.com/betterlll/Multi-Resolution-SAR-dataset-


### SARptical数据集
光学图像的分辨率为 0.2m，SAR 图像的分辨率为 1m。

图像尺寸：112×112 像素

数据集中的每对图像块的中心像素在三维空间中的位置被精确匹配，精度通常在 几米范围内。

示例图片: 

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

示例图片: 

<img width="850" alt="392be66bab033c4046d890336774b9f" src="https://github.com/user-attachments/assets/5df37b7d-0a48-43ea-9c87-3f0ddeafbbac" />

SEN1-2数据集下载链接: https://dataserv.ub.tum.de/index.php/s/m1436631

### SARBuD 1.0 数据集
SARBuD 1.0（SAR Building Dataset）是一个面向深度学习的中高分辨率 SAR 建筑数据集，由中国科学院空天信息创新研究院基于高分三号（GF-3）卫星的精细模式单极化 SAR 影像构建。

SARBuD 1.0 数据集包含 60,000 张 256×256 像素的有效建筑区样本切片，以及 80,000 张覆盖多种其他地物类型的负样本切片。

SARBuD 1.0 数据集基于 GF-3 卫星的精细模式单极化 SAR 影像，分辨率为 10m。

数据集涵盖中国不同区域的多种地形场景类型和分布类型，包括大面积聚集城区和小范围山区乡镇。

所有建筑区样本均通过高分辨率光学图像手动标注。

示例图片: 

![image](https://github.com/user-attachments/assets/e9625d8e-b8c6-4320-8c41-03bf036c8ea7)

SARBuD 1.0 数据集下载链接: https://github.com/CAESAR-Radi/SARBuD

### YeSeg数据集
YESeg-OPT-SAR 使用的是 2010 年 10 月 21 日至 2016 年 8 月 25 日期间谷歌地球 L18 产品所拍摄的高分辨率光学和 SAR 图像，其空间分辨率为 0.5 米。

该数据集包含 2231 对相同区域的图像，每张图像的大小为 256×256。

数据集涵盖两个研究区域，一个位于东经 122.836° 至 122.869°、北纬 45.105° 至 45.133° 的范围内，另一个位于东经 110.135° 至 110.160°、北纬 34.593° 至 34.626° 的范围内，涵盖了不同地形和植被的广泛区域。

研究区域的位置在下面的地图中有所标注。

<img width="750" alt="1750471445362" src="https://github.com/user-attachments/assets/a7cfed6c-00ac-42ab-b2c4-877339bc6baa" />

数据集中的图像已全部以像素级别进行了分类标注，包括背景、裸地、植被、树木、房屋、水体、道路及其他类别，其中标签值和各类别所占百分比见下表。

| Label  |  Name  | Percent(%) |
|--------|--------|------------|
| 0 | background | 2.26 |
| 1 | bareground | 55.84 |
| 2 | low vegetation | 26.55 |
| 3 | trees | 5.29 |
| 4 | houses | 4.39 |
| 5 | water | 1.69 |
| 6 | roads | 3.88 |
| 7 | other | 0.11 |

示例图片: 

<img width="700" alt="1750471487990" src="https://github.com/user-attachments/assets/7f88b19d-7f5a-425e-86fe-c6c42c2df92f" />

YESeg数据集下载链接: https://github.com/yeyuanxin110/YESeg-OPT-SAR

### OS-Eval数据集
OS-Eval 数据集是一个高分辨率的光学和 SAR 图像配准评估数据集。该数据集包含数百对亚米级分辨率的光学和 SAR 图像，并使用在光学和 SAR 图像中具有清晰结构的元极作为地面真值，以定量评估光学和 SAR 配准算法。

OS-Eval数据集分为相对数据集和绝对数据集两部分：

- 相对数据集

OPT+RPC+GT：包含 tiff 图像、RPC 文件和对应的 GT 文件（无地理编码）。

SAR+RPC+GT：包含 tiff 图像、RPC 文件和对应的 GT 文件（斜距，无地理编码）。

OMH_USGS10m_WGS84.tif：10 米分辨率的 DEM（WGS84）。

OMHdsm.tif：0.5 米分辨率的 DSM（WGS84）。

Processed：使用 DEM/DSM 进行地理编码的图像。 OPT-ORG-DEM：使用 DEM 进行地理编码的 tiff 图像（1 米 GSD，WGS84）。 SAR-ORG-DEM：使用 DEM 进行地理编码的 tiff 图像（1 米 GSD，WGS84）。 OPT-ORG-DSM：使用 DSM 进行地理编码的 tiff 图像（1 米 GSD，WGS84）。 SAR-ORG-DSM：使用 DSM 进行地理编码的 tiff 图像（1 米 GSD，WGS84）。

shp：来自 OpenStreetMap 的建筑物 shapefile（1 米 GSD，WGS84）。

Meta：11 个光学产品和 13 个 SAR 产品的元文件。

- 绝对数据集

Google+GT：包含来自 Google Earth 的正射 tiff 图像和对应的 GT 文件（WGS84）。

SAR+RPC+GT：包含 tiff 图像、RPC 文件和对应的 GT 文件（斜距，无地理编码）。

ZZG_USGS10m_WGS84.tif：10 米分辨率的 DEM（WGS84）。

ZZGdsm.tif：0.5 米分辨率的 DSM（WGS84）。

Processed：使用 DEM/DSM 进行地理编码的图像。 OPT：调整到 1 米 GSD 的正射 tiff 图像（WGS84）。 SAR-ORG-DEM：使用 DEM 进行地理编码的 tiff 图像（1 米 GSD，WGS84）。 SAR-ORG-DSM：使用 DSM 进行地理编码的 tiff 图像（1 米 GSD，WGS84）。

shp：来自 OpenStreetMap 的建筑物 shapefile（1 米 GSD，WGS84）。

Meta：19 个 SAR 产品的元文件。

示例图片: 

![image](https://github.com/user-attachments/assets/78266465-3dc2-4e35-b766-28d843c51999)


os-eval数据集下载链接: https://github.com/xym2009/OS-Eval?tab=readme-ov-file

### WHU OPT SAR数据集
WHU-OPT-SAR 包含了 RGB 图像、近红外（NIR）光学图像以及相应的 SAR 图像，覆盖面积达 51448.56 平方公里，分辨率为 5 米。

利用高分一号（GF-1）卫星的光学影像与高分三号（GF-3）卫星在同一区域的SAR影像，构建了大尺度光学SAR联合土地利用分类数据集WHU-OPT-SAR。

WHU-OPT-SAR数据集包含 100 幅 5556*3704 像素的光学图像和相同区域的SAR图像，覆盖中国湖北省（30°N-33°N, 108°E-117°E）约50000 km2的区域。该地区属亚热带季风气候，最低海拔50米，最高海拔3000米。

WHU-OPT-SAR覆盖了广泛的山地、林地、丘陵、平原等不同地形和针叶林、阔叶林、灌木、水生植被等不同植被的遥感影像。

该数据集中带有像素级标注的图像可以为基于深度学习的土地利用分类提供数据源。其训练良好的模型可用于训练遥感领域的其他类似任务。

示例图片: 

<img width="650" alt="1750473379504" src="https://github.com/user-attachments/assets/9bd937e9-276f-4ab1-93c8-34fe2e013daa" />

WHU-OPT-SAR数据集相关介绍: https://github.com/AmberHen/WHU-OPT-SAR-dataset

百度网盘下载链接: https://pan.baidu.com/s/1sIGsD3lBEogSCqzbDOaclA  密码: i51o

谷歌云盘下载链接: https://drive.google.com/drive/folders/1W3iMpkehng7ADXmhz9pPvmgFQBayq22t?usp=sharing

参考文献: https://www.sciencedirect.com/science/article/pii/S0303243421003457?via%3Dihub

### SAR2Opt Heterogeneous数据集
SAR 图像由 TerraSAR-X 传感器获取，光学图像来自 Google Earth Engine。SAR 图像采集自 2007 年至 2013 年，覆盖亚洲、北美洲、大洋洲和欧洲的十个城市的高分辨率区域。

训练集包含 1450 对 600×600 的 SAR 和 RGB 光学图像，测试集包含 627 对。

SAR 图像的空间分辨率为 1 米，所有图像块在配准后裁剪为 600×600 像素。

数据集可用于训练和测试多种基于 GAN 的图像翻译方法，如 Pix2Pix、CycleGAN、MUNIT 等。

示例图片: 

![image](https://github.com/user-attachments/assets/89a3ea06-a552-4699-970a-1d41d021558c)
![image](https://github.com/user-attachments/assets/23465849-0763-4357-8afa-da7e7e753abd)

SAR2Opt Heterogeneous数据集相关介绍: https://github.com/MarsZhaoYT/SAR2Opt-Heterogeneous-Dataset

百度网盘下载链接: https://pan.baidu.com/share/init?surl=xQ1nc2aPFdJ99SI2upl5Tg  密码: hy8d

谷歌云盘下载链接: https://drive.google.com/file/d/1XB9pWq-tVdxQsbVALxbYIF0Em90J4kkR/view

参考文献: https://ieeexplore.ieee.org/document/9779739

### QXS-SAROPT数据集
QXS-SAROPT数据集包含 20,000 对 SAR-光学图像片段，SAR 和光学图像的空间分辨率均为 1米。

原始图像块尺寸为 600×600 像素。为了便于使用，图像被裁剪为 256×256 像素 的小块

从高分三号卫星的 SAR 卫星图像中获取 SAR 片段，从谷歌地球获取光学片段。这些图像覆盖了三个港口城市：圣地亚哥、上海和青岛。

在此，对数据集的构建进行了详细的介绍，并展示了其两个具有代表性的典型应用，即 SAR-光学图像匹配以及借助光学图像的跨模态信息增强的 SAR 船只检测。

作为一个具有多个高分辨率场景的大型开放 SAR-光学数据集， QXS-SAROPT 对基于深度学习的 SAR-光学数据融合技术的进一步研究具有潜在价值。

示例图片: 

![image](https://github.com/user-attachments/assets/df460536-af74-4410-9a9c-86c2cea31b9c)

QXS-SAROPT数据集下载链接: https://github.com/yaoxu008/QXS-SAROPT?tab=readme-ov-file

参考文献: https://arxiv.org/pdf/2103.08259

### University1652-Baseline
University1652-Baseline包含来自全球72所大学1 652座建筑的地面影像、模拟生成的无人机视角影像和卫星影像3种平台的数据。

相关介绍链接：https://github.com/layumi/University1652-Baseline

参考文献: https://arxiv.org/abs/2002.12186

### OS-dataset
OS-Dataset 是一个高分辨率的光学和SAR图像配准数据集，由 Xiang 等人在2020年创建。

该数据集包含10692对图像（训练集8044对，验证集952对，测试集1696对），图像大小为256×256像素，主要包含城市、河流、农田地表起伏不大的场景。

其中SAR图像来源于高分三号，分辨率为1m。

光学图像收集于谷歌地球平台，并重新采样到1m分辨率。

OS-Dataset 数据集具有空间分辨率高、空间分布广、地物类型丰富等优点，且可通过数据增强进一步提升数据样本量。

示例图片: 

![image](https://github.com/user-attachments/assets/a8b007c2-4dcc-4acf-a16e-9ca0503e0b9c)

OS-dataset数据集相关介绍: https://github.com/xym2009/OSdataset/blob/main/README.md

百度网盘下载链接: https://pan.baidu.com/s/14bqaJhMSZEy7EXcXVAc77w?pwd=vriw

谷歌云盘下载链接: https://drive.google.com/file/d/10gySGfj0-pH1N2TeZWYU1H38OskzKC27/view?usp=sharing

### SOPatch数据集
SOPatch数据集是一个用于深度学习的稀疏SAR（合成孔径雷达）与光学图像匹配的框架的一部分。

它主要用于研究和开发SAR与光学图像之间的匹配技术，特别是在遥感领域。该框架结合了深度学习技术，旨在解决SAR和光学图像之间的特征差异问题，从而实现高效的图像匹配。

基于3个数据集WHU-SEN-City、OSdataset和 SEN1-2，共创建包含超过65万对的光学和SAR配准数据集。SOPatch数据集的空间分辨率包括10米和1米。

示例图片: 

<img width="575" alt="1750488285893" src="https://github.com/user-attachments/assets/08965601-0dc8-47c1-808b-a2e9024ccfd2" />

SOPatch数据集下载链接：https://github.com/system123/SOMatch

参考文献: https://doaj.org/article/5a379cf911f546dab596f3324e9370ca
## 非遥感数据集

### Brown数据集
Brown数据集是一个图像匹配的经典集合，包含了Liberty、NotreDame和Yosemite三个地方的图像。数据集通过三维重建获取特征点信息和匹配关系，常用于图像处理和计算机视觉研究。

Brown数据集由 1024 x 1024 位图 (.bmp) 图像组成，每个图像包含一个 16 x 16 图像块阵列。每个补丁都被采样为 64 x 64 灰度，具有规范的比例和方向。

示例图片: 

![image](https://github.com/user-attachments/assets/21667115-ec5a-4bb1-9ac4-cbc0ab81578a)

参考文献: https://ieeexplore.ieee.org/document/9850980

Brown数据集下载链接: https://phototour.cs.washington.edu/patches/default.htm

### MD-syn数据集
MD-syn数据集是由华中科技大学和武汉大学联合创建的多模态图像匹配数据集。它旨在解决跨模态图像匹配中的数据稀缺问题，通过生成模型从RGB图像扩展而来，包含多种模态（如RGB、红外、深度等）和丰富场景。

MD-syn数据集包含七种模态类型，包括RGB、红外、深度、事件、法线图、草图和绘画，广泛应用于跨模态图像匹配任务，显著提升了模型的泛化能力和零样本性能。

该数据集包含4.8亿对图像，继承了RGB数据的匹配标签和多样性。

数据集的图像分辨率未明确提及，但其源数据来自MegaDepth数据集，该数据集的图像分辨率通常为1024×768像素。

数据集的幅宽（图像宽度）未明确提及，但基于MegaDepth数据集的图像宽度通常为1024像素。

示例图片: 

![image](https://github.com/user-attachments/assets/e492e996-8f17-4716-8637-a969e4e66de9)

MD-syn数据集下载链接: https://github.com/LSXI7/MINIMA

参考文献: https://arxiv.org/abs/2412.19412
### Multimodal Image Matching Datasets
Multimodal Image Matching Datasets数据库包含了 18 种常见的数据类型，并且这些数据都有真实值标注。

从这些收集到的原始图像对中，研究者手动为每一对标注了 15 到 20 个匹配的地标点（即位置点），这些点可用于根据这些匹配的地标点之间的距离来评估配准的准确性。

研究者还为一些图像对提供了仿射变换矩阵（那些本质上进行线性变换的图像对），以便通过使用这些给定的仿射矩阵，能够很好地进行配准而不会出现任何明显的错位。

基于每个图像对的变换矩阵，可以知道在固定图像和移动图像中哪两个点是匹配的，并判断由特征描述符创建的匹配点是否正确。

示例图片: 

![image](https://github.com/user-attachments/assets/f383d6f6-3356-41f2-8f3b-d4a9e2bbd989)

MD-syn数据集下载链接: https://github.com/StaRainJ/Multi-modality-image-matching-database-metrics-methods

参考文献: https://doi.org/10.1016/j.inffus.2021.02.012 
