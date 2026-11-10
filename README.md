# 🦌 Hjort-YOLO: Lightweight and Explainable Wildlife Detection

**A lightweight, efficient, and explainable deep learning framework for wildlife detection using camera-trap images.**

📄 **Published in:** Frontiers in Artificial Intelligence (2026)

🔗 **Research Paper:** https://doi.org/10.3389/frai.2026.1930016

## Overview

Hjort-YOLO is an optimized object detection framework built upon YOLOv11n, designed to detect wildlife efficiently in challenging natural environments.

The framework addresses key challenges in automated wildlife monitoring, including complex forest backgrounds, partial occlusion, variable lighting conditions, and computational limitations.

Our research focuses on achieving a balance between **detection accuracy, computational efficiency, and model explainability**, making the approach promising for real-time wildlife monitoring and resource-constrained applications.

## Key Contributions

- **Lightweight architecture:** Modified YOLOv11n with optimized C2f-W and A2C2f-W modules and a reduced detection head.
- **Improved computational efficiency:** Approximately 19% fewer GFLOPs compared with YOLOv11n.
- **Faster wildlife detection:** Improved inference performance while maintaining competitive detection accuracy.
- **Explainable AI:** Integrated Grad-CAM and Captum for visualizing image regions influencing model predictions.
- **Wildlife segmentation:** Incorporated SAM2 for pixel-level segmentation of detected animals.
- **Evaluation across datasets:** Validated using the Svanøy deer dataset from Norway and the African Wildlife dataset.


## Datasets
## Svanøy Deer Dataset
The dataset contains camera-trap imagery collected on Svanøy Island, Norway, including day and night observations of red deer.

## African Wildlife Dataset
The dataset includes:

Buffalo
Elephant
Rhino
Zebra
Please refer to the original sources for dataset licensing and access.



## Experimental Results

On the Svanøy deer dataset, Hjort-YOLO demonstrated the following performance compared with YOLOv11n:

| Metric | YOLOv11n | Hjort-YOLO |
|---|---:|---:|
| mAP@50 | 0.979 | 0.981 |
| GFLOPs | 6.4 | 5.1 |
| Inference time | 8.0 ms | 6.8 ms |
| FPS | 21.98 | 24.98 |
| Model parameters | 2.59M | 2.90M |

These results demonstrate that architectural optimization can improve inference efficiency without sacrificing detection accuracy at mAP@50.

## Potential Applications

- Automated wildlife monitoring
- Camera-trap image analysis
- Biodiversity conservation
- Edge-based wildlife detection
- Future wildlife–vehicle collision warning systems

## Citation

If you find this research useful, please cite:

Momin, M. A., Khan, M., Arghandeh, R., Bischof, R., Hegland, S. J., Moen, T., & Stølen, M. F. (2026). *Hjort-YOLO: A lightweight and explainable computer vision framework for wildlife detection.* Frontiers in Artificial Intelligence, 9, 1930016.

https://doi.org/10.3389/frai.2026.1930016


or,

If you use Hjort-YOLO in your research, please cite:

@article{momin2026hjortyolo,
  title={Hjort-YOLO: A Lightweight and Explainable Computer Vision Framework for Wildlife Detection},
  author={Momin, Md Abdul and Khan, Mehak and Arghandeh, Reza and Bischof, Richard and Hegland, Stein Joar and Moen, Terje and Stølen, Martin F.},
  journal={Frontiers in Artificial Intelligence},
  volume={9},
  pages={1930016},
  year={2026},
  doi={10.3389/frai.2026.1930016}
}


## Acknowledgment
This work was conducted under the WILDETECT project and supported by the Research Council of Norway (Project No. 344408), in collaboration with:

Western Norway University of Applied Sciences (HVL)
Norwegian Institute for Nature Research (NINA)
SINTEF
Norwegian Public Roads Administration (NPRA)
IMSA Knowledge Company


## Contact
Md Abdul Momin (PhD student)
Western Norway University of Applied Sciences (HVL)
📧 momin.md.abdul@hvl.no
