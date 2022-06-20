# ChiSig Dataset Release

[Paper Link](https://openaccess.thecvf.com/content/CVPR2022W/SketchDL/papers/Yan_Signature_Detection_Restoration_and_Verification_A_Novel_Chinese_Document_Signature_CVPRW_2022_paper.pdf)

We construct a novel Chinese document offline signature forgery detection benchmark, namely `ChiSig`, which includes all tasks, i.e., signature detection, restoration, and verification.

* Download Link: 

## Description

Currently, a Chinese signature dataset that can be obtained is [ICDAR 2011 Signature Verification Competition (SigComp2011) - TC11](http://www.iapr-tc11.org/mediawiki/index.php/ICDAR_2011_Signature_Verification_Competition_(SigComp2011)). However, the dataset has limited data, with only 1177 signature images and 20 different names for offline signature verification. Unlike existing datasets, ours has 10,242 images with 500 different signed names.

![sample images for signatures](image/sample-image.png)

## Dataset Construction

The dataset consists of clean handwritten signatures, synthesized noisy handwritten signatures, and synthesized documents with handwritten signatures.

We randomly generate 500 names and then let volunteers sign according to certain rules to get the clean signature data, which can be used for signature verification tasks. Then, we obtain scanned documents that can be used to synthesize backgrounds through public resources, such as [XFUND dataset](https://github.com/doc-analysis/XFUND), Chinese National Standards and patents. We randomly place the signatures in the background documents, so that we can obtain data that can be used for signature detection and signature reconstruction.

For the time being, we only publish the signature data and the corresponding mask that we have obtained, users can obtain the background documents and perform document synthesis by themselves.

We may update our data in the future to improve its diversity

![dataset setting](image/dataset-setting.png)

## Benchmark

The dataset includes three benchmarks, detection, restoration, and verification. The selected evaluation methods are all strong baselines and representative methods in the related fields. In addition, the stability and robustness of the selected methods have been verified. Details for each
task are provided in our [paper](https://openaccess.thecvf.com/content/CVPR2022W/SketchDL/papers/Yan_Signature_Detection_Restoration_and_Verification_A_Novel_Chinese_Document_Signature_CVPRW_2022_paper.pdf).

![result](image/result.png)


## Citation and Contact

Please consider to cite our paper when you use our dataset. 

**Note**: The dataset can only be used for non-commercial purposes

```
@InProceedings{Yan_2022_CVPR,
    author    = {Yan, Kaihong and Zhang, Ying and Tang, Haoran and Ren, Chengkai and Zhang, Jian and Wang, Gaoang and Wang, Hongwei},
    title     = {Signature Detection, Restoration, and Verification: A Novel Chinese Document Signature Forgery Detection Benchmark},
    booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) Workshops},
    month     = {June},
    year      = {2022},
    pages     = {5163-5172}
}
```

For any questions about this database please contact the author below.

```
Dr. Jian Zhang
E-mail: jianzhang@intl.zju.edu.cn
```
