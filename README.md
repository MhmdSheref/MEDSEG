# MEDSEG
A medical segmentation and visualization utility notebook for comparing the results of 3 different AI models

<a target="_blank" href="https://colab.research.google.com/drive/1fbPTDlPnLo8WgzaxAVzAGZ7thVWc6hVa?usp=sharing">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

### Brief
This project was created by Cairo University Systems and Biomedical Engineering students under the strict deadline of 2 weeks.
Its main goal is to accept CT input and return a segmentation of body organs using 3 different AI models as well as 3D visualization of the organs.
We were also asked to evaluate the 3 AI models' accuracy.

## How to use
Run the code blocks sequentially, giving input when asked to do so by widgets. **(This notebook is intended for use in a T4 GPU Runtime)**

The notebook comes with a sample of CT scans taken from [TotalSegmentator](https://github.com/wasserth/TotalSegmentator/)'s [CT Dataset](https://zenodo.org/records/10047292). that can be used for testing and evaulation.


## Features
1. CT image viewer for reviewing the scan before segmentation
2. Three Different AI models to choose from for inference
    - [TotalSegmentator](https://github.com/wasserth/TotalSegmentator/)
    - [MONAI SegResNet Whole Body CT Segmentation](https://monai.io/model-zoo.html#/model/wholeBody_ct_segmentation)
    - [STU-Net](https://github.com/uni-medical/STU-Net)
3. Accurate 3D visualization of segmented body parts with options for color, opacity, and visability.
4. Evaluation using multiple metrics
     - Dice Similarity Coefficient
     - Jaccard Index
     - Hausdorff Distance
6. Visualization and analysis of the results.



## Acknowledgements
- TotalSegmentator:
```
Wasserthal, J., Breit, H.-C., Meyer, M.T., Pradella, M., Hinck, D., Sauter, A.W., Heye, T., Boll, D., Cyriac, J., Yang, S., Bach, M., Segeroth, M., 2023. TotalSegmentator: Robust Segmentation of 104 Anatomic Structures in CT Images. Radiology: Artificial Intelligence. https://doi.org/10.1148/ryai.230024
```

- nnU-Net:
```
Isensee, F., Jaeger, P. F., Kohl, S. A., Petersen, J., & Maier-Hein, K. H. (2021). nnU-Net: a self-configuring 
method for deep learning-based biomedical image segmentation. Nature methods, 18(2), 203-211.
```

- STU-Net:
```
@misc{huang2023stunet,
      title={STU-Net: Scalable and Transferable Medical Image Segmentation Models Empowered by Large-Scale Supervised Pre-training}, 
      author={Ziyan Huang and Haoyu Wang and Zhongying Deng and Jin Ye and Yanzhou Su and Hui Sun and Junjun He and Yun Gu and Lixu Gu and Shaoting Zhang and Yu Qiao},
      year={2023},
      eprint={2304.06716},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```

- SegResNet:
```
Myronenko, A., Siddiquee, M.M.R., Yang, D., He, Y. and Xu, D., 2022. Automated head and neck tumor segmentation from 3D PET/CT. arXiv preprint arXiv:2209.10809.
```

- MONAI
```
Tang, Y., Gao, R., Lee, H.H., Han, S., Chen, Y., Gao, D., Nath, V., Bermudez, C., Savona, M.R., Abramson, R.G. and Bao, S., 2021. High-resolution 3D abdominal segmentation with random patch network fusion. Medical image analysis, 69, p.101894.
```
