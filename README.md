# Groundtruth of spliced images in dataset CASIA 2.0

* CASIA 1.0 groundtruth dataset is avaiable at: https://github.com/namtpham/casia1groundtruth

* Groundtruth dataset can be downloaded directly from this repository.
* Recently, I received several requests of the original dataset since the server is no longer available.
I upload this dataset to my Drive to spread this dataset to the research community. Please visit the following link to download: (~2.6 GB)

* [Update 2021/04/20] Revised dataset: https://bit.ly/2QazgkG

I removed the download link of the original dataset to avoid the confusion. If you need it, feel free to email me.

* [Update 2019/09/30]: In this version, almost the noises in the previous version are handled. The file names are also revised carefully.

* [List of duplicate authentic images](https://pastebin.com/BBdwR3cX) provided by another researcher.

Please notice that the authors made many mistakes in naming the files. People who download the original dataset (before 2021/04/20) please rename the tampered images using the commands in the excel files. 
Originally, it was reported that there are 5123 tampered images, including 3274 copy-move images and 1849 spliced images. However, mistakenly classified files are renamed as follows.

| No. of images | Originally named as           | Re-classified as              |
| :---:         | :---:                         | :---:                         |
| 39            | Copy-move images (TP_S_)      | Spliced images (S->D)         |
| 60            | Spliced images (TP_D_)        | Copy-move images (D->S)       |

        After renaming the files, the number of copy-move and spliced images are 3295 and 1828, respectively.

Due to the lack of manual file, I write up here the naming convention:

## Authentic images:

Au_ani_00001.jpg
Au: Authentic
ani: animal category
Other categories: arc (architecture), art, cha (characters), ind (indoor), nat (nature), pla (plants), txt (texture)

## Tampering images

a. Spliced image

        Tp_D_CRN_S_N_cha00063_art00014_11818.jpg
* Tp: Tampering
* D: Different (means the tampered region was copied from the different image)
* Next 5 letters stand for the techniques they used to create the images. Unfortunately, I don't remember exactly.
* cha00063: the source image
* art00014: the target image
* 11818: tampered image ID

b. Copy-move images

        Tp_S_NRN_M_N_pla00020_pla00020_10988.jpg
* Tp: Tampering
* S: Same (means the tampered region was copied from the same image)
* And the rest is similar to case a.

If you use the groundtruth dataset for a scientific publication, please cite the following paper:

    @article{pham2019hybrid,
      title={Hybrid Image-Retrieval Method for Image-Splicing Validation},
      author={Pham, Nam Thanh and Lee, Jong-Weon and Kwon, Goo-Rak and Park, Chun-Su},
      journal={Symmetry},
      volume={11},
      number={1},
      pages={83},
      year={2019},
      publisher={Multidisciplinary Digital Publishing Institute}
    }
