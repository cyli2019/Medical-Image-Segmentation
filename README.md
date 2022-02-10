# Medical Image Segmentation

*Last updated: 02/09/2022*

## Most Interested

| Date                                                                      | First Author  | Title                                                    | Architecture | Modality                                    | ND   | Loss                                             | Dataset                                                                                                              | Code                                                   | Paper                                                                                                              |
| ------------------------------------------------------------------------- | ------------- | -------------------------------------------------------- | ------------ | ------------------------------------------- | ---- | ------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ |
| 10/08/2021                                                                | Jiacheng Wang | Boundary-aware Transformers for Skin Lesion Segmentation | Transformer  | Image                                       | 2D   | CE+Dice with boundary-wise prior knowledge       | ISIC 2016 + PH2, ISIC 2018                                                                                           | [PyTorch](https://github.com/jcwang123/BA-Transformer) | MICCAI 2021 [![arXiv](https://img.shields.io/badge/arXiv-2103.14030-b31b1b.svg)](https://arxiv.org/abs/2110.03864) |
| 07/10/2021                                                                | Li Lin        | BSDA-Net: A Boundary Shape and Distance Aware Joint Learning Framework for Segmenting and Classifying OCTA Images | CNN           | Image                                                    | 2D           | MSE with soft label heatmap on the boundary | OCTA | [PyTorch](https://github.com/llmir/MultitaskOCTA) | MICCAI 2021 [![arXiv](https://img.shields.io/badge/arXiv-2010.11929-b31b1b.svg)](https://arxiv.org/abs/2107.04823) |                                                        |                                                                                                                    |
| 06/10/2019                                                                | Hoel Kervadec  | Boundary loss for highly unbalanced segmentation | CNN           | MRI                                                    | 2D/3D          | CE+B | WMH  | [PyTorch](https://github.com/LIVIAETS/boundary-loss) | MIDL 2019 [![arXiv](https://img.shields.io/badge/arXiv-2010.11929-b31b1b.svg)](https://arxiv.org/abs/1812.07032) |                                                        |                                                                                                                    |
| 06/01/2020                                                                | Jun Ma  | How Distance Transform Maps Boost Segmentation CNNs: An Empirical Study | CNN           | CT/MRI                                                    | 3D          | Dice+ B/HD/SDF | MICCAI 2017, 2018 | [PyTorch](https://github.com/LIVIAETS/surface-los) | MIDL 2020 [![arXiv](https://img.shields.io/badge/arXiv-2010.11929-b31b1b.svg)](http://proceedings.mlr.press/v121/ma20b/ma20b.pdf) |                                                        |                                                                                                                    |


## Image Segmentation with Transformer

| Date         | First Author               | Title                                                                                                           | Modality                    | ND      | Loss                                                     | Dataset                                                           | Code                                                                                      | Paper                                                                                                              |
| ------------ | -------------------------- | --------------------------------------------------------------------------------------------------------------- | --------------------------- | ------- | -------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| 01/26/2022   | Shiqi Huang                | RTNet: Relation Transformer Network for Diabetic Retinopathy Multi-lesion Segmentation                          | DR (Image)                  | 2D      | CE (Multi-class weighted)                                | IDRiD and DDR                                                     | N/A                                                                                       | IEEE TMI [![arXiv](https://img.shields.io/badge/arXiv-2201.11037-b31b1b.svg)](https://arxiv.org/abs/2201.11037)    |
| D01/04/2022  | Ali Hatamizadeh            | Swin UNETR: Swin Transformers for Semantic Segmentation of Brain Tumors in MRI Images                           | MRI                         | 3D      | Dice                                                     | BraTS 2021 (1251 subjects, semantic segmentation of brain tumors) | [PyTorch](https://github.com/Project-MONAI/research-contributions/tree/master/SwinUNETR)  | [![arXiv](https://img.shields.io/badge/arXiv-2201.01266-b31b1b.svg)](https://arxiv.org/abs/2201.01266)             |
| ()01/03/2022 | Yixuan Wu                  | D-Former: A U-shaped Dilated Transformer for 3D Medical Image Segmentation                                      | MRI & CT                    | 3D      | CE + Dice                                                | Synapse (multi-organ segmentation) and ACDC (cardiac diagnosis)   | N/A                                                                                       | [![arXiv](https://img.shields.io/badge/arXiv-2201.00462-b31b1b.svg)](https://arxiv.org/abs/2201.00462)             |
| 12/09/2021   | Xiangde Luo                | Semi-Supervised Medical Image Segmentation via Cross Teaching between CNN and Transformer                       | MRI                         | 2D      | Dice                                                     | ACDC                                                              | [PyTorch](https://github.com/HiLab-git/SSL4MIS)                                           | [![arXiv](https://img.shields.io/badge/arXiv-2112.04894-b31b1b.svg)](https://arxiv.org/abs/2112.04894)             |
| 11/29/2021   | Yucheng Tang               | Self-Supervised Pre-Training of Swin Transformers for 3D Medical Image Analysis                                 | CT & MRI                    | 3D      | Inpaint + Constrast coding + rotation (for pre-training) | 5 CT scan datasets                                                | [PyTorch](https://monai.io/research/swin-unetr)                                           | [![arXiv](https://img.shields.io/badge/arXiv-2111.14791-b31b1b.svg)](https://arxiv.org/abs/2111.14791)             |
| 11/26/2021   | Himashi Peiris             | A Volumetric Transformer for Accurate 3D Tumor Segmentation                                                     | CT & MRI                    | 3D      | CE+Dice                                                  | BraTS                                                             | [PyTorch](https://github.com/himashi92/VT-UNet)                                           | [![arXiv](https://img.shields.io/badge/arXiv-2111.13300-b31b1b.svg)](https://arxiv.org/abs/2111.13300)             |
| 11/15/2021   | Dong Yang                  | T-AutoML: Automated Machine Learning for Lesion Segmentation using Transformers in 3D Medical Imaging           | CT                          | 3D      | CE+Dice                                                  | LiTS 2017, Medical Segmentation Decathlon                         | N/A                                                                                       | ICCV 2021 [![arXiv](https://img.shields.io/badge/arXiv-2111.07535-b31b1b.svg)](https://arxiv.org/abs/2111.07535)   |
| 11/08/2021   | Hongyi Wang                | Mixed Transformer U-Net For Medical Image Segmentation                                                          | CT                          | 2D      | CE/Dice                                                  | Synapse, ACDC                                                     | [PyTorch](https://github.com/Dootmaan/MT-UNet)                                            | [![arXiv](https://img.shields.io/badge/arXiv-2111.04734-b31b1b.svg)](https://arxiv.org/abs/2111.04734)             |
| 09/15/2021   | Xiaohong Huang             | MISSFormer: An Effective Medical Image Segmentation Transformer                                                 | CT                          | 2D      | CE+Dice                                                  | Synapse, ACDC                                                     | [PyTorch](https://github.com/ZhifangDeng/MISSFormer)                                      | [![arXiv](https://img.shields.io/badge/arXiv-2109.07162-b31b1b.svg)](https://arxiv.org/abs/2109.07162)             |
| 09/07/2021   | Hong-Yu Zhou               | nnFormer: Interleaved Transformer for Volumetric Segmentation                                                   | CT                          | 3D      | CE+Dice                                                  | Synapse, ACDC                                                     | [PyTorch](https://github.com/282857341/nnFormer)                                          | [![arXiv](https://img.shields.io/badge/arXiv-2109.03201-b31b1b.svg)](https://arxiv.org/abs/2109.03201v1)           |
| 07/28/2021   | Madeleine K. Wyburd        | TEDS-Net: Enforcing Diffeomorphisms in Spatial Transformers to Guarantee Topology Preservation in Segmentations | MRI                         | 2D      | Dice+Flow Feild Regularisation                           | ACDC                                                              | [PyTorch](https://github.com/mwyburd/TEDS-Net)                                            | MICCAI 2021 [![arXiv](https://img.shields.io/badge/arXiv-2107.13542-b31b1b.svg)](https://arxiv.org/abs/2107.13542) |
| 07/19/2021   | Guoping Xu                 | LeViT-UNet: Make Faster Encoders with Transformer for Medical Image Segmentation                                | CT                          | 2D      | CE+Dice                                                  | Synapse, ACDC                                                     | N/A                                                                                       | [![arXiv](https://img.shields.io/badge/arXiv-2107.08623-b31b1b.svg)](https://arxiv.org/abs/2107.08623)             |
| 07/12/2021   | Bingzhi Chen               | TransAttUnet: Multi-level Attention-guided U-Net with Transformer for Medical Image Segmentation                | X-ray & CT ...              | 2D      | CE+Dice                                                  | ISIC-2018, JSRT ...                                               | N/A                                                                                       | [![arXiv](https://img.shields.io/badge/arXiv-2107.05274-b31b1b.svg)](https://arxiv.org/abs/2107.05274)             |
| 07/12/2021   | Chang Yao                  | TransClaw U-Net: Claw U-Net with Transformers for Medical Image Segmentation                                    | CT                          | 2D      | CE                                                       | Synapse                                                           | N/A                                                                                       | [![arXiv](https://img.shields.io/badge/arXiv-2107.05188-b31b1b.svg)](https://arxiv.org/abs/2107.05188)             |
| 07/02/2021   | Yunhe Gao                  | UTNet: A Hybrid Transformer Architecture for Medical Image Segmentation                                         | CT                          | 2D      | CE+Dice                                                  | [M&Ms dataset](https://www.ub.edu/mnms/)                          | [PyTorch](https://github.com/yhygao/UTNet)                                                | MICCAI 2021 [![arXiv](https://img.shields.io/badge/arXiv-2107.00781-b31b1b.svg)](https://arxiv.org/abs/2107.00781) |
| 06/28/2021   | Yuanfeng Ji                | Multi-Compound Transformer for Accurate Biomedical Image Segmentation                                           | Colonoscopy & Pathology ... | 2D      | CE+Dice+auxiliary loss                                   | Six segmentation datasetsc ...                                    | [PyTorch](https://github.com/JiYuanFeng/MCTrans)                                          | MICCAI 2021 [![arXiv](https://img.shields.io/badge/arXiv-2106.14385-b31b1b.svg)](https://arxiv.org/abs/2106.14385) |
| 06/12/2021   | Ailiang Lin                | DS-TransUNet: Dual Swin Transformer U-Net for Medical Image Segmentation                                        | Colonoscopy & Histology ... | 2D      | IoU+CE                                                   | Four seg datasets ...                                             | N/A                                                                                       | [![arXiv](https://img.shields.io/badge/arXiv-2106.06716-b31b1b.svg)](https://arxiv.org/abs/2106.06716)             |
| 06/02/2021   | Shaohua Li                 | Medical Image Segmentation Using Squeeze-and-Expansion Transformers                                             | Fundus &  Colonoscopy & MRI | 2D & 3D | CE+Dice                                                  | REFUGE20, Polyp, BraTS19                                          | [PyTorch](https://github.com/askerlee/segtran)                                            | IJCAI 2021 [![arXiv](https://img.shields.io/badge/arXiv-2105.09511-b31b1b.svg)](https://arxiv.org/abs/2105.09511)  |
| 05/12/2021   | Hu Cao                     | Swin-Unet: Unet-like Pure Transformer for Medical Image Segmentation                                            | CT                          | 2D      | CE+Dice                                                  | Synapse                                                           | [PyTorch](https://github.com/HuCaoFighting/Swin-Unet)                                     | [![arXiv](https://img.shields.io/badge/arXiv-2105.05537-b31b1b.svg)](https://arxiv.org/abs/2105.05537)             |
| 03/18/2021   | Ali Hatamizadeh            | UNETR: Transformers for 3D Medical Image Segmentation                                                           | CT & MRI                    | 3D      | CE+Dice                                                  | BTCV                                                              | [PyTorch](https://github.com/Project-MONAI/research-contributions/tree/master/UNETR/BTCV) | [![arXiv](https://img.shields.io/badge/arXiv-2103.10504-b31b1b.svg)](https://arxiv.org/abs/2103.10504)             |
| 03/10/2021   | Olivier Petit              | U-Net Transformer: Self and Cross Attention for Medical Image Segmentation                                      | CT                          | 2D      | Dice                                                     | TCIA, IMO                                                         | N/A                                                                                       | [![arXiv](https://img.shields.io/badge/arXiv-2103.06104-b31b1b.svg)](https://arxiv.org/abs/2103.06104)             |
| 03/07/2021   | Wenxuan Wang               | TransBTS: Multimodal Brain Tumor Segmentation Using Transformer                                                 | MRI                         | 3D      | Dice                                                     | BraTS 2019                                                        | [PyTorch](https://github.com/Wenxuan-1119/TransBTS)                                       | MICCAI 2021 [![arXiv](https://img.shields.io/badge/arXiv-2103.04430-b31b1b.svg)](https://arxiv.org/abs/2103.04430) |
| 03/04/2021   | Yutong Xie                 | CoTr: Efficiently Bridging CNN and Transformer for 3D Medical Image Segmentation                                | CT                          | 3D      | CE+Dice                                                  | BCV                                                               | [PyTorch](https://github.com/YtongXie/CoTr)                                               | MICCAI 2021[![arXiv](https://img.shields.io/badge/arXiv-2103.03024-b31b1b.svg)](https://arxiv.org/abs/2103.03024)  |
| 02/21/2021   | Jeya Maria Jose Valanarasu | Medical Transformer: Gated Axial-Attention for Medical Image Segmentation                                       | Ultrasound & Microscopic    | 2D      | CE                                                       | Brain US, GlaS, MoNuSeg                                           | [PyTorch](https://github.com/jeya-maria-jose/Medical-Transformer)                         | MICCAI 2021 [![arXiv](https://img.shields.io/badge/arXiv-2102.10662-b31b1b.svg)](https://arxiv.org/abs/2102.10662) |

## Transformer fundamental papers

| Date       | First Author       | Title                                                                      | Code                                                                                                              | Paper                                                                                                            |
| ---------- | ------------------ | -------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| 03/25/2021 | Ze Liu             | Swin Transformer: Hierarchical Vision Transformer using Shifted Windows    | [PyTorch](https://github.com/microsoft/Swin-Transformer)                                                          | [![arXiv](https://img.shields.io/badge/arXiv-2103.14030-b31b1b.svg)](https://arxiv.org/abs/2103.14030)           |
| 10/22/2020 | Alexey Dosovitskiy | An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale | [JAX](https://github.com/google-research/vision_transformer) [PyTorch](https://github.com/jeonsworld/ViT-pytorch) | ICLR 2020 [![arXiv](https://img.shields.io/badge/arXiv-2010.11929-b31b1b.svg)](https://arxiv.org/abs/2010.11929) |
| 12/06/2017 | Ashish Vaswani     | Attention Is All You Need                                                  | [TensorFlow](https://github.com/tensorflow/tensor2tensor)                                                         | NIPS 2017 [![arXiv](https://img.shields.io/badge/arXiv-1706.03762-b31b1b.svg)](https://arxiv.org/abs/1706.03762) |
