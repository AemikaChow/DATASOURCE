# DATASOURCE for *fAshIon* :thought_balloon:

This is a **summary**. We reviewed all  (to our best knowledge) fashion-related papers in the past decade and recorded the datasets had been used. The numbers to describe the dataset is faithfully followed its original paper. The webpage is organized as:  

The sections are defined according to the types of data, *e.g.* if you want clothing segmentation information, you can see Section 0. parsing to find annotated data.  

If you want to obtain some attributes, you can see Section 1. attribute. We present the type of attributes (*e.g.* brand, review, style, comment, neckline, color *etc*), the number of images, potential tasks, type of images (*e.g.* product image, model image, which view, *etc*) for a quick check.  

:pig: means the dataset can be found. If you find the dataset helpful, please kindly cite it in your paper ("bibtex" is offered for your convenience)~  

Meanwhile, for consistency, we uniformed the words decribe the fashion concept.
- &nbsp;**Silhouette** (shape, cut, fit): the shape of a garment, *e.g.* H line, A line *etc*;
- &nbsp;**Material** (fabric): the material made a garment, *e.g.* chiffon, lace *etc*;
- &nbsp;**Print** (pattern, texture): the surface design of a garment, *e.g.* checks, dotted *etc*;
- &nbsp;**Neckline** (collar shape, collar): the design in the neck region of a garment, *e.g.* V-neck, lapel *etc*; 
- &nbsp;**Design details** (structures, style): designs which can be used in anywhere of a garment, *e.g.* frilly, ruffled *etc*;
- &nbsp;**Opening** (cloth button, fastening): the way designed in the opening of a garment *e.g.* button, zipped *etc*;
- &nbsp;**Category** (type): type of a garment, *e.g.* dress, top *etc*;
- &nbsp;**Sub-category**: fine-grained type of a garment, *e.g.* wedding dress, T-shire *etc*;
- &nbsp;**Styles** (looks): the expressed feeling of a garment of an outfit, *e.g.* lovely, casual *etc*;
- &nbsp;**Gender** (Persons): Men's wear, women's wear (child, boy, female) *etc*;
- &nbsp;**Design Attributes**: the attributes used in the process of garment design, *e.g.* shirt cuff, shirt collar *etc*;
- &nbsp;**Retail Attributes**: the attributes used in the process of retail, *e.g.*  parka, windbreaker *etc*.  

If you have problems with a specific dataset shows below, please kindly contact its authors. For a quick check, you can also see my own [memo version](https://drive.google.com/open?id=1ucwMgee0Df1P--cDHQR9XdcPPuMjgaSt) &copy;

<!-- toc -->

- [0. &nbsp;Parsing](#0-parsing)
- [1. &nbsp;Keypoints](#1-keypoints)
- [2. &nbsp;Attribute](#2-attribute)
- [3. &nbsp;Outfit](#3-outfit)
- [4. &nbsp;Generation](#4-generation)
- [5. &nbsp;Others](#5-others)
- [Other Sources](#other-sources)
- [Acknowledge](#acknowledge)

<!-- tocstop -->

## 0. &nbsp;Parsing 
For semantic segmentation, object detection, instance segmentation, polygon detection, and *etc*.
*****
:cherries: **Fashionista 2012**   

(1) **158,235** fashion photos with associated text annotations (tags, comments, and links).  
(2) The tags are noisy or incomplete.  
(3) **685** photos with good visibility of the full-body with pose annotations for the usual 14 body parts.  
(4) There are totally **56** labels (**53** category or sub-category labels, and additional labels for hair, skin, and null (background).  

[[homepage]](http://vision.is.tohoku.ac.jp/~kyamagu/research/clothing_parsing/) [[pdf]](http://vision.is.tohoku.ac.jp/~kyamagu/papers/yamaguchi_cvpr2012.pdf) :pig:
```bib
@inproceedings{yamaguchi2012parsing,
  title={Parsing clothing in fashion photographs},
  author={Yamaguchi, Kota and Kiapour, M Hadi and Ortiz, Luis E and Berg, Tamara L},
  booktitle={2012 IEEE Conference on Computer Vision and Pattern Recognition},
  pages={3570--3577},
  year={2012},
  organization={IEEE}
}
```
  
  
:cherries: **Paperdoll 2013**   

(1) Over **1 million** pictures from chictopia.com with associated metadata tags i.e. color, clothing item, or occasion.  
(2) **339,797** pictures weakly annotated with clothing items and estimated pose.  
(3) **685** fully parsed images .

[[homepage]](http://vision.is.tohoku.ac.jp/~kyamagu/research/paperdoll/) [[pdf]](https://www.cv-foundation.org/openaccess/content_iccv_2013/papers/Yamaguchi_Paper_Doll_Parsing_2013_ICCV_paper.pdf) :pig:
```bib
@inproceedings{yamaguchi2013paper,
  title={Paper doll parsing: Retrieving similar styles to parse clothing items},
  author={Yamaguchi, Kota and Hadi Kiapour, M and Berg, Tamara L},
  booktitle={Proceedings of the IEEE international conference on computer vision},
  pages={3519--3526},
  year={2013}
}
```


:cherries: **CFPD 2013**   

(1) **97,490** images with 292,541 tags from Chictopia.com.  
(2) **2,682** images in total, and all the pixels in the images are annotated with both color labels (**13**) and category labels (**23**).   
(3) **Weakly supervised setting**, where only image-level tags are available in the training phase.

[homepage] [[pdf]](https://liusi-group.com/pdf/Fashion%20Parsing%20With%20Weak%20Color-Category%20Labels.pdf) [[github1]](https://github.com/zbxzc35/dataset-CFPD) [[github2]](https://github.com/hrsma2i/dataset-CFPD) :pig:
```bib
@article{liu2013fashion,
  title={Fashion parsing with weak color-category labels},
  author={Liu, Si and Feng, Jiashi and Domokos, Csaba and Xu, Hui and Huang, Junshi and Hu, Zhenzhen and Yan, Shuicheng},
  journal={IEEE Transactions on Multimedia},
  volume={16},
  number={1},
  pages={253--265},
  year={2013},
  publisher={IEEE}
}
```


:cherries: **CCP 2013**     

(1) It consisting of **2098** high-resolution street fashion photos.  
(2) More than **1,000** images are annotated with superpixel-level labeling with a total of **57** tags.  
(3) Cross-scenario image pairs, which include about **10,000** product photos and user's photos image pairs.   
(4) Each image has **124** fine-grained semantic attributes.  
(5) **20** categories, **56** colors, **6** clothing length, **10** silhouette, **25** necklines, and **7** sleeve length. 
 
[[homepage]](http://www.sysu-hcp.net/clothing-co-parsing-by-joint-image-segmentation-and-labeling/) [[pdf]](http://linliang.net/wp-content/uploads/2017/07/TMM_Clothes.pdf) [[github]](https://github.com/bearpaw/clothing-co-parsing) :pig:
```bib
@inproceedings{yang2014clothing,
  title={Clothing Co-Parsing by Joint Image Segmentation and Labeling},
  author={Yang, Wei and Luo, Ping and Lin, Liang}
  booktitle={Computer Vision and Pattern Recognition (CVPR), 2014 IEEE Conference on},
  year={2013},
  organization={IEEE}
}
```


:cherries: **HCP 2015**   

(1) **7,700** images in total.  
(2) Combined Fashionista (685), CFPD (2,682), Daily Photos dataset (2,500).  
(3) Crawl another **1,833** challenging images （*e.g.* sitting or occlusion) annotate pixel-level labels.  
(4) **18** categories of labels, *e.g.*  face, sunglass, hat, scarf *etc*.  

[[homepage]](http://www.sysu-hcp.net/clothing-co-parsing-by-joint-image-segmentation-and-labeling/) [[pdf]](https://arxiv.org/pdf/1503.02391.pdf) :pig:
```bib
@article{liang2015deep,
  title={Deep human parsing with active template regression},
  author={Liang, Xiaodan and Liu, Si and Shen, Xiaohui and Yang, Jianchao and Liu, Luoqi and Dong, Jian and Lin, Liang and Yan, Shuicheng},
  journal={IEEE transactions on pattern analysis and machine intelligence},
  volume={37},
  number={12},
  pages={2402--2414},
  year={2015},
  publisher={IEEE}
}
```


:cherries: **Fashion Icon 2015** 

(1) **Video dataset** and **Fashion Icon (FI) image dataset**.  
(2) Video dataset contains **1, 500** videos.  
(3) FI image dataset contains **1, 082** images, **18** categories.  

[homepage] [[pdf]](https://liusi-group.com/pdf/Fashion%20Parsing%20with%20Video%20Context.pdf)
```bib
@article{liu2015fashion,
  title={Fashion parsing with video context},
  author={Liu, Si and Liang, Xiaodan and Liu, Luoqi and Lu, Ke and Lin, Liang and Cao, Xiaochun and Yan, Shuicheng},
  journal={IEEE Transactions on Multimedia},
  volume={17},
  number={8},
  pages={1347--1358},
  year={2015},
  publisher={IEEE}
}
```


:cherries: **Refined Fashionista 2017**   

(1) Reduces the number of clothing categories from **56** to **25** essential labels.  
(2) Manually annotated all the **685** images in the Fashionista dataset.  

[[homepage]](http://vision.is.tohoku.ac.jp/~kyamagu/research/clothing_parsing/) [[pdf]](https://arxiv.org/pdf/1703.01386.pdf) [[github]](https://github.com/pongsate1/fashion-parsing) :pig:
```bib
@article{tangseng2017looking,
  title={Looking at outfit to parse clothing},
  author={Tangseng, Pongsate and Wu, Zhipeng and Yamaguchi, Kota},
  journal={arXiv preprint arXiv:1703.01386},
  year={2017}
}
```


:cherries: **FASHION8 2018**   

(1) **9,339** fashion images from **8** continuous years are collected.  
(2) With human-annotated foreground masks.  

[homepage] [[pdf]](https://arxiv.org/pdf/1803.03415.pdf)
```bib
@article{zhang2018fusing,
  title={Fusing Hierarchical Convolutional Features for Human Body Segmentation and Clothing Fashion Classification},
  author={Zhang, Zheng and Song, Chengfang and Zou, Qin},
  journal={arXiv preprint arXiv:1803.03415},
  year={2018}
}
```


:cherries: **ModaNet 2018**  

(1) **55, 176** street images, fully annotated with polygons (bounding box, segmentation mask).  
(2) Based on 1 million weakly annotated street images in **Paperdoll**.  
(3) **13** categories annotated (*e.g.* bag, belt, boots).  

[[homepage]](https://github.com/eBay/modanet) [[pdf]](https://arxiv.org/pdf/1807.01394.pdf) [[github]](https://github.com/hrsma2i/modanet) :pig:
```bib
@inproceedings{zheng2018modanet,
  title={Modanet: A large-scale street fashion dataset with polygon annotations},
  author={Zheng, Shuai and Yang, Fan and Kiapour, M Hadi and Piramuthu, Robinson},
  booktitle={Proceedings of the 26th ACM international conference on Multimedia},
  pages={1670--1678},
  year={2018}
}
```


## 1. &nbsp;Keypoints
For keypoint detection, landmark detection, pose estimation and *etc*.
*****
:cherries: **FLD 2016**  

(1) Over **120K** images.  
(2) Each image is correctly labeled with **8** fashion landmarks along with their visibility.  
(3) Different types of clothing items, including upper/lower/full-body clothes.  
(4) Different subsets, including normal/medium/large poses and medium/large scales.  

[[homepage]](http://mmlab.ie.cuhk.edu.hk/projects/DeepFashion/LandmarkDetection.html) [[pdf]](https://arxiv.org/pdf/1608.03049.pdf) [[github]](https://github.com/liuziwei7/fashion-landmarks) :pig:
```bib
@inproceedings{liu2016fashionlandmark,
 author = {Ziwei Liu, Sijie Yan, Ping Luo, Xiaogang Wang, and Xiaoou Tang},
 title = {Fashion Landmark Detection in the Wild},
 booktitle = {European Conference on Computer Vision (ECCV)},
 month = {October},
 year = {2016} 
}
```


:cherries: **FASHIONAI Keypoint 2018**  

(1) **24** key points in **324k** image (including armpit, crotch keypoints).  

[[homepage]](https://tianchi.aliyun.com/competition/entrance/231648/introduction?lang=zh-cn) [[pdf]](http://openaccess.thecvf.com/content_CVPRW_2019/papers/FFSS-USAD/Zou_FashionAI_A_Hierarchical_Dataset_for_Fashion_Understanding_CVPRW_2019_paper.pdf) [[TIANCHI]](https://tianchi.aliyun.com/competition/entrance/231670/introduction?spm=5176.12281949.1003.9.493e1dc1qVUD4c) :pig:

:orange: You may kindly obtain the data by logging in to the TIANCHI platform (Choosing the international version, then register a personal account and sign the agreement. You will be supposed to access the data successfully).
```bib
@inproceedings{zou2019fashionai,
  title={FashionAI: A Hierarchical Dataset for Fashion Understanding},
  author={Zou, Xingxing and Kong, Xiangheng and Wong, Waikeung and Wang, Congde and Liu, Yuguang and Cao, Yang},
  booktitle={Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition Workshops},
  pages={0--0},
  year={2019}
}
```
:cherries: **DeepFashion2 2019**  

(1) **801K** clothing items annotated with style, scale, viewpoint, occlusion, bounding box, dense landmarks, masks.  
(2) **873K** Commercial-Consumer clothes pairs.  
(3) **13** different definitions of landmarks and poses for **13** different categories.  

[homepage] [[pdf]](https://arxiv.org/pdf/1901.07973.pdf) [[github]](https://github.com/switchablenorms/DeepFashion2) :pig:
```bib
@article{DeepFashion2,
  author = {Yuying Ge and Ruimao Zhang and Lingyun Wu and Xiaogang Wang and Xiaoou Tang and Ping Luo},
  title={A Versatile Benchmark for Detection, Pose Estimation, Segmentation and Re-Identification of Clothing Images},
  journal={CVPR},
  year={2019}
}
```


## 2. &nbsp;Attribute
For style analysis, attribute recognition, trend anaylsis, style anaylsis, multi-task learning, consumer-to-shop clothes retrieval, in-shop clothes retrieval and *etc*.
*****
:cherries: **Apparel Style 2012**  

(1) **15** categories (*e.g.* Long dress, Coat, Jacket *etc*).  
(2) Over **80, 000** images.  
(3) Attributes including colors(13), print(15), material(8), design details(4), styles(4+21), gender(5), sleeve length(3).  

[[homepage]](https://data.vision.ee.ethz.ch/cvl/lbossard/accv12/) [[pdf]](https://data.vision.ee.ethz.ch/cvl/lbossard/accv12/accv12_apparel-classification-with-style.pdf) :pig:
```bib
@inproceedings{bossard2012apparel,
  title={Apparel classification with style},
  author={Bossard, Lukas and Dantone, Matthias and Leistner, Christian and Wengert, Christian and Quack, Till and Van Gool, Luc},
  booktitle={Asian conference on computer vision},
  pages={321--335},
  year={2012},
  organization={Springer}
}
```


:cherries: **WFC 2013**  

(1) **Women’s Coat** Dataset contains **2,092** images total with manuly annotated labels.  
(2) **12** coat/jacket categories: cape, military, motorcycle, peacoat, poncho, puffer, trench, *etc*.  
(3) **27** (Material(5), Fastener(4), Fastener style(3),  clothing length(3), silhouette(2), pocket(2), neckline(8)) binary attributes.  

[homepage] [[pdf]](https://www.cv-foundation.org/openaccess/content_cvpr_workshops_2013/W03/papers/Di_Style_Finder_Fine-Grained_2013_CVPR_paper.pdf)
```bib
@inproceedings{di2013style,
  title={Style finder: Fine-grained clothing style detection and retrieval},
  author={Di, Wei and Wah, Catherine and Bhardwaj, Anurag and Piramuthu, Robinson and Sundaresan, Neel},
  booktitle={Proceedings of the IEEE Conference on computer vision and pattern recognition workshops},
  pages={8--13},
  year={2013}
}
```


:cherries: **ZOZOTOWN 2013**  

(1) **12,719** photos on  ZOZOTOWN.  
(2) Have several meta-data, gender information,  wearing items information, and photo date.  

[homepage] [[pdf]](https://www.researchgate.net/profile/Kiyoharu_Aizawa/publication/261438969_SNAPPER_Fashion_coordinate_image_retrieval_system/links/0f31753472d15b5839000000/SNAPPER-Fashion-coordinate-image-retrieval-system.pdf)
```bib
@inproceedings{miura2013snapper,
  title={SNAPPER: fashion coordinate image retrieval system},
  author={Miura, Shinya and Yamasaki, Toshihiko and Aizawa, Kiyoharu},
  booktitle={2013 International Conference on Signal-Image Technology \& Internet-Based Systems},
  pages={784--789},
  year={2013},
  organization={IEEE}
}
```


:cherries: **Fashion136K 2013**  

(1) **135,893** street fashion images with annotations by fashionistas, brand, demographics.  
(2) **3-4** annotations per image.  

[homepage] [[pdf]](https://dl.acm.org/doi/pdf/10.1145/2623330.2623332)
```bib
@inproceedings{jagadeesh2014large,
  title={Large scale visual recommendations from street fashion images},
  author={Jagadeesh, Vignesh and Piramuthu, Robinson and Bhardwaj, Anurag and Di, Wei and Sundaresan, Neel},
  booktitle={Proceedings of the 20th ACM SIGKDD international conference on Knowledge discovery and data mining},
  pages={1925--1934},
  year={2014}
}
```


:cherries: **UT-Zap50K 2014**  

(1) **50,000 shoe** images with fine-grained attributes.  
(2) **4** relative attributes: “open”, “pointy at the toe”, “sporty”, and “comfortable".  
(3) **12,000** total pairs, 3,000 per attribute.  

[[homepage]](http://vision.cs.utexas.edu/projects/finegrained/utzap50k/) [[pdf]](http://aronyu.io/vision/papers/cvpr14/aron-cvpr14.pdf) :pig:
```bib
@InProceedings{finegrained,
  author = {A. Yu and K. Grauman},
  title = {Fine-Grained Visual Comparisons with Local Learning},
  booktitle = {Computer Vision and Pattern Recognition (CVPR)},
  month = {Jun},
  year = {2014}
}
```


:cherries: **Fashion 10000 2014**  

(1) **32,398** photos, with their associated metadata, distributed in **262** diﬀerent fashion categories.  

[[homepage]](http://traces.cs.umass.edu/index.php/Mmsys/Mmsys) [[pdf]](https://dl.acm.org/doi/pdf/10.1145/2557642.2563675) :pig:
```bib
@inproceedings{loni2014fashion,
  title={Fashion 10000: an enriched social image dataset for fashion and clothing},
  author={Loni, Babak and Cheung, Lei Yen and Riegler, Michael and Bozzon, Alessandro and Gottlieb, Luke and Larson, Martha},
  booktitle={Proceedings of the 5th ACM Multimedia Systems Conference},
  pages={41--46},
  year={2014}
}
```


:cherries: **Hipster Wars 2014**  

(1) **1,893** images labeled with **5 style** categories: hipster, bohemian, pinup, preppy, and goth.  

[homepage] [[pdf]](https://projet.liris.cnrs.fr/imagine/pub/proceedings/ECCV-2014/papers/8689/86890472.pdf)
```bib
@inproceedings{kiapour2014hipster,
  title={Hipster wars: Discovering elements of fashion styles},
  author={Kiapour, M Hadi and Yamaguchi, Kota and Berg, Alexander C and Berg, Tamara L},
  booktitle={European conference on computer vision},
  pages={472--488},
  year={2014},
  organization={Springer}
}
```


:cherries: **Fashion144K 2015**  

(1) **144,169** user posts containing diverse images, textual, and meta information.  
(2) Labels like location, comments, votes *etc*.  

[[homepage]](https://esslab.jp/~ess/en/data/fashion144k_stylenet/) [[pdf]](https://www.cs.toronto.edu/~urtasun/publications/simo_etal_cvpr15.pdf) :pig:
```bib
@InProceedings{SimoSerraCVPR2015,
  author    = {Edgar Simo-Serra and Sanja Fidler and Francesc Moreno-Noguer and Raquel Urtasun},
  title     = {{Neuroaesthetics in Fashion: Modeling the Perception of Fashionability}},
  booktitle = "Proceedings of the Conference on Computer Vision and Pattern Recognition (CVPR)",
  year      = 2015,
}
```


:cherries: **WITB(Exact Street2Shop) 2015**  

(1) **404,683** shop photos and **20,357** street photos.  
(2) Providing a total of **39,479** clothing item matches.  

[[homepage]](http://www.tamaraberg.com/street2shop/) [[pdf]](http://www.tamaraberg.com/papers/street2shop.pdf) :pig:
```bib
@inproceedings{hadi2015buy,
  title={Where to buy it: Matching street clothing photos in online shops},
  author={Hadi Kiapour, M and Han, Xufeng and Lazebnik, Svetlana and Berg, Alexander C and Berg, Tamara L},
  booktitle={Proceedings of the IEEE international conference on computer vision},
  pages={3343--3351},
  year={2015}
}
```

:cherries: **DARN 2015**  

(1)  **453,983** online upper-clothing images with **179** attributes in high-resolution.  
(2) Each image contains a single frontal-view person.  
(3) Opening(12), Category(20), Color(56), Cloth length(6), Print(27), Silhouette(10), Neckline(25), Sleeve length(7), Sleeve shape(16).  

[homepage] [[pdf]](https://www.cv-foundation.org/openaccess/content_iccv_2015/papers/Huang_Cross-Domain_Image_Retrieval_ICCV_2015_paper.pdf)
```bib
@inproceedings{huang2015cross,
  title={Cross-domain image retrieval with a dual attribute-aware ranking network},
  author={Huang, Junshi and Feris, Rogerio S and Chen, Qiang and Yan, Shuicheng},
  booktitle={Proceedings of the IEEE international conference on computer vision},
  pages={1062--1070},
  year={2015}
}
```


:cherries: **Clothing1M 2015**  

(1)  **1, 000, 000** clothing images with 14 class labels: T-shirt, Shirt, Knitwear, Chiffon, Sweater, Hoodie *etc*.  
(2) Each image is automatically assigned with a noisy label according to the keywords in its surrounding text.  
(3) Manually refine **72, 409** image labels, which constitute a clean sub-dataset.  

[homepage] [[pdf]](https://www.ee.cuhk.edu.hk/~xgwang/papers/xiaoXYHWcvpr15.pdf) [[github]](https://github.com/Cysu/noisy_label) :pig:
```bib
@inproceedings{xiao2015learning,
  title={Learning from Massive Noisy Labeled Data for Image Classification},
  author={Xiao, Tong and Xia, Tian and Yang, Yi and Huang, Chang and Wang, Xiaogang},
  booktitle={CVPR},
  year={2015}
}
```


:cherries: **YahooClothing 2015**  

(1)  **161,234** fashion images in the Yahoo shopping dataset.  
(2) It labeled with category, gender, and sub-category(15) such as Top, Dress, Coat *etc*.  

[homepage] [[pdf]](https://dl.acm.org/doi/pdf/10.1145/2671188.2749318)
```bib
@inproceedings{lin2015rapid,
  title={Rapid clothing retrieval via deep learning of binary codes and hierarchical search},
  author={Lin, Kevin and Yang, Huei-Fang and Liu, Kuan-Hsien and Hsiao, Jen-Hao and Chen, Chu-Song},
  booktitle={Proceedings of the 5th ACM on International Conference on Multimedia Retrieval},
  pages={499--502},
  year={2015}
}
```


:cherries: **Chitopia 2015**  

(1) Chictopia dataset has **26,8124** usable images, each image has **2** clothing-keywords under **18** categories.  
(2) Dress dataset consists of **712** images with total of **58** attributes.  

[homepage] [[pdf]](http://www.bmva.org/bmvc/2015/papers/paper051/paper051.pdf)
```bib
@inproceedings{yamaguchi2015mix,
  title={Mix and Match: Joint Model for Clothing and Attribute Recognition.},
  author={Yamaguchi, Kota and Okatani, Takayuki and Sudo, Kyoko and Murasaki, Kazuhiko and Taniguchi, Yukinobu},
  booktitle={BMVC},
  volume={1},
  number={2},
  pages={4},
  year={2015}
}
```


:cherries: **Etsy | Wear 2016**  

(1) Etsy dataset has **173,175** clothing products.  
(2) Wear dataset has **212,129** images associated shots from different views, list of items, blog text, tags, and other metadata.  

[[homepage]](http://vision.is.tohoku.ac.jp/~kyamagu/research/etsy-dataset/) [[pdf]](https://arxiv.org/pdf/1607.07262.pdf) :pig:
```bib
@inproceedings{vittayakorn2016automatic,
  title={Automatic attribute discovery with neural activations},
  author={Vittayakorn, Sirion and Umeda, Takayuki and Murasaki, Kazuhiko and Sudo, Kyoko and Okatani, Takayuki and Yamaguchi, Kota},
  booktitle={European Conference on Computer Vision},
  pages={252--268},
  year={2016},
  organization={Springer}
}
```


:cherries: **DeepFashion 2016**  

(1) Over **800,000** images, which are richly annotated with massive attributes, clothing landmarks, and correspondence of images.  
(2) **50** fine-grained categories and **1, 000 descriptive attributes**.  
(3) Attributes including Category,  Print, Material, Silhouette, Part, Style.  

[[homepage]](http://mmlab.ie.cuhk.edu.hk/projects/DeepFashion.html) [[pdf]](https://www.ee.cuhk.edu.hk/~xgwang/papers/liuLQWTcvpr16.pdf) :pig:
```bib
@inproceedings{liuLQWTcvpr16DeepFashion,
 author = {Liu, Ziwei and Luo, Ping and Qiu, Shi and Wang, Xiaogang and Tang, Xiaoou},
 title = {DeepFashion: Powering Robust Clothes Recognition and Retrieval with Rich Annotations},
 booktitle = {Proceedings of IEEE Conference on Computer Vision and Pattern Recognition (CVPR)},
 month = {June},
 year = {2016} 
 }
 ```
 
 
:cherries: **MVC 2016**  

(1) **37,499** items and **161,638** clothing images, **264** attributes(gender, category, sub-catgegory, design attributes).  
(2)  Multi-view(front, back, right, left) with high-resolution.  

[[homepage]](http://mvc-datasets.github.io/MVC/) [[pdf]](https://www.iis.sinica.edu.tw/papers/song/19692-F.pdf) [[github]](https://github.com/MVC-Datasets/MVC) :pig:
```bib
@inproceedings{liu2016mvc,
  title={Mvc: A dataset for view-invariant clothing retrieval and attribute prediction},
  author={Liu, Kuan-Hsien and Chen, Ting-Yen and Chen, Chu-Song},
  booktitle={Proceedings of the 2016 ACM on International Conference on Multimedia Retrieval},
  pages={313--316},
  year={2016}
}
```


:cherries: **StreetStyle27K 2017**  

(1) **27K** images, each with **12** clothing attributes.  
(2) A first-of-its-kind analysis of global and per-city fashion choices and trends.  
(3) 7 binary attributes(Wearing Jacket, Wearing Scarf *etc*), 13 colors, 7 categories, 3 sleeve length, 3 neckline, 6 print.  

[[homepage]](http://streetstyle.cs.cornell.edu/#dataset) [[pdf]](https://arxiv.org/pdf/1706.01869.pdf) :pig:
```bib
@article{StreetStyle2017,
  title={{StreetStyle}: {E}xploring world-wide clothing styles from millions of photos},
  author={Kevin Matzen and Kavita Bala and Noah Snavely},
  journal={arXiv preprint arXiv:1706.01869},
  year={2017}
}
```


:cherries: **Fashionstyle14 2017**  

(1) **13,126** images labeled with **14** different fashion styles (conservative, dressy, ethnic, fairy, feminine *etc*).  

[[homepage]](https://esslab.jp/~ess/en/data/fashionstyle14/) [[pdf]](http://openaccess.thecvf.com/content_ICCV_2017_workshops/papers/w32/Takagi_What_Makes_a_ICCV_2017_paper.pdf) :pig:
```bib
@inproceedings{takagi2017makes,
  title={What makes a style: Experimental analysis of fashion prediction},
  author={Takagi, Moeko and Simo-Serra, Edgar and Iizuka, Satoshi and Ishikawa, Hiroshi},
  booktitle={Proceedings of the IEEE International Conference on Computer Vision Workshops},
  pages={2247--2253},
  year={2017}
}
```


:cherries: **Fashion200K 2017**  

(1) Over **200,000** images of five categories (dress, top, pants, skirt, and jacket) and their product descriptions.  
(2) After dealing with product description, **4,404** attributes(words) have remained.  

[homepage] [[pdf]](http://openaccess.thecvf.com/content_ICCV_2017/papers/Han_Automatic_Spatially-Aware_Fashion_ICCV_2017_paper.pdf) [[github]](https://github.com/xthan/fashion-200k/) :pig:
```bib
@inproceedings{han2017automatic,
  title = {Automatic Spatially-aware Fashion Concept Discovery},
  author = {Han, Xintong and Wu, Zuxuan and Huang, Phoenix X. and Zhang, Xiao and Zhu, Menglong and Li, Yuan and Zhao, Yang  and Davis, Larry S.},
  booktitle = {ICCV},
  year  = {2017},
}
```


:cherries: **Fashion550K 2017**  

(1) **weakly-labeled** image dataset consists of **550,661** images that includes **5,300** human-annotated images.  
(2) **66** binary labels, 26 colors, 22 categories, 7 shoes, 11 accessories.  

[[homepage]](https://esslab.jp/~ess/en/data/fashion550k/) [[pdf]](http://openaccess.thecvf.com/content_ICCV_2017_workshops/papers/w32/Inoue_Multi-Label_Fashion_Image_ICCV_2017_paper.pdf) :pig:
```bib
@InProceedings{InoueICCVW2017,
   author    = {Naoto Inoue and Edgar Simo-Serra and Toshihiko Yamasaki and Hiroshi Ishikawa},
   title     = {{Multi-Label Fashion Image Classification with Minimal Human Supervision}},
   booktitle = "Proceedings of the International Conference on Computer Vision Workshops (ICCVW)",
   year      = 2017,
}
```


:cherries: **Amazon Dress**  

(1) **53 689** images of dresses and their product descriptions.  
(2) Different categories, such as bridesmaid, casual, mother of the bride, night out and cocktail, and wedding.  
(3) The product descriptions consist of the surrounding natural language text, like the title, features, and editorial content.  

[homepage] [[pdf]](https://kddfashion2017.mybluemix.net/final_submissions/ML4Fashion_paper_7.pdf)
```bib
@inproceedings{laenen2017cross,
  title={Cross-modal search for fashion attributes},
  author={Laenen, Katrien and Zoghbi, Susana and Moens, Marie-Francine},
  booktitle={Proceedings of the KDD 2017 Workshop on Machine Learning Meets Fashion},
  volume={2017},
  pages={1--10},
  year={2017},
  organization={ACM}
}
```


:cherries: **SFS 2017**  

(1) **293,105** posts, each image consists of weakly-labeled multi-task ground-truth.  
(2) Labels including season, occasion, fashion style, garment categories, geographical and year information.  

[[homepage]](https://zenodo.org/record/833051#.XqfGivmWa70) [[pdf]](http://doi.org/10.1145/3123266.3123441) :pig:
```bib
@inproceedings{gu2017understanding,
  title={Understanding fashion trends from street photos via neighbor-constrained embedding learning},
  author={Gu, Xiaoling and Wong, Yongkang and Peng, Pai and Shou, Lidan and Chen, Gang and Kankanhalli, Mohan S},
  booktitle={Proceedings of the 25th ACM international conference on Multimedia},
  pages={190--198},
  year={2017}
}
```


:cherries: **Video2Shop 2017**  

(1) **26,352** clothing trajectories extracted from 526 videos and **85,677** clothing shopping images.  
(2) **14** categories of clothes are manually labeled.  

[homepage] [[pdf]](http://openaccess.thecvf.com/content_cvpr_2017/papers/Cheng_Video2Shop_Exact_Matching_CVPR_2017_paper.pdf)
```bib
@inproceedings{cheng2017video2shop,
  title={Video2shop: Exact matching clothes in videos to online shopping images},
  author={Cheng, Zhi-Qi and Wu, Xiao and Liu, Yang and Hua, Xian-Sheng},
  booktitle={Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition},
  pages={4048--4056},
  year={2017}
}
```


:cherries: **RFS | PFS 2018**  

  

[homepage] [[pdf]]  
```bib
@article{gu2018multi,
  title={Multi-Modal and Multi-Domain Embedding Learning for Fashion Retrieval and Analysis},
  author={Gu, Xiaoling and Wong, Yongkang and Shou, Lidan and Peng, Pai and Chen, Gang and Kankanhalli, Mohan S},
  journal={IEEE Transactions on Multimedia},
  volume={21},
  number={6},
  pages={1524--1537},
  year={2018},
  publisher={IEEE}
}
```


:cherries: **BrandFashion 2018**  

(1) **10K** clothing images with distinctive logos from **15** brands.  
(2) Label with **16** clothing categories and **32** semantic attributes.  

[homepage] [[pdf]](http://openaccess.thecvf.com/content_ECCVW_2018/papers/11131/Manandhar_Tiered_Deep_Similarity_Search_for_Fashion_ECCVW_2018_paper.pdf)
```bib
@inproceedings{manandhar2018tiered,
  title={Tiered Deep Similarity Search for Fashion},
  author={Manandhar, Dipu and Bastan, Muhammet and Yap, Kim-Hui},
  booktitle={Proceedings of the European Conference on Computer Vision (ECCV)},
  pages={0--0},
  year={2018}
}
```

:cherries: **FashionBrand 2018**  

(1) **3,828,735** clothing product images from **1,219** brands.   
(2) Attributes including 5 categories, 13 sub-categories.  

[homepage] [[pdf]](https://arxiv.org/pdf/1810.09941v1.pdf)
```bib
@inproceedings{hadi2018brand,
  title={Brand> Logo: Visual Analysis of Fashion Brands},
  author={Hadi Kiapour, M and Piramuthu, Robinson},
  booktitle={Proceedings of the European Conference on Computer Vision (ECCV)},
  pages={0--0},
  year={2018}
}
```
:cherries: **Fashion60 2018**  

(1) **539,704** images for training and **30, 000** images for testing.  
(2) **60** fine-grained fashion attributes categorized into 5 coarse-grained groups.  

[homepage] [[pdf]](https://ieeexplore.ieee.org/document/8396968)
```bib
@inproceedings{kuang2018ontology,
  title={Ontology-driven hierarchical deep learning for fashion recognition},
  author={Kuang, Zhenzhong and Yu, Jun and Yu, Zhou and Fan, Jianping},
  booktitle={2018 IEEE Conference on Multimedia Information Processing and Retrieval (MIPR)},
  pages={19--24},
  year={2018},
  organization={IEEE}
}
```
:cherries: **X-domain 2018**  

(1) **245,467** shop images. Each image is annotated by **9** attribute labels.  
(2) Imbalanced with an **imbalance-ratio** of 1:4,162 (20 : 204,177).  
(3) **178** distinctive attributes over the 9 labels, including 6 sleeve-length, 55 colors.  

[homepage] [[pdf]](https://arxiv.org/pdf/1804.10851.pdf)
```bib
@article{dong2018imbalanced,
  title={Imbalanced deep learning by minority class incremental rectification},
  author={Dong, Qi and Gong, Shaogang and Zhu, Xiatian},
  journal={IEEE transactions on pattern analysis and machine intelligence},
  volume={41},
  number={6},
  pages={1367--1381},
  year={2018},
  publisher={IEEE}
}
```


:cherries: **Women | Men Video 2018**  

(1) Video dataset **for unsupervised learning**.  
(2) Two new clothing image datasets are annotated with **10** pre-defined clothing attributes.  
(3) **18,737** woman clothing videos and **21,224** man clothing videos.  

[homepage] [[pdf]](https://www.researchgate.net/profile/Sanyi_Zhang/publication/321785076_Watch_Fashion_Shows_to_Tell_Clothing_Attributes/links/5cdf0e3c92851c4eabaa3e07/Watch-Fashion-Shows-to-Tell-Clothing-Attributes.pdf)
```bib
@article{zhang2018watch,
  title={Watch fashion shows to tell clothing attributes},
  author={Zhang, Sanyi and Liu, Si and Cao, Xiaochun and Song, Zhanjie and Zhou, Jie},
  journal={Neurocomputing},
  volume={282},
  pages={98--110},
  year={2018},
  publisher={Elsevier}
}
```
:cherries: **FASHIONAI Attributes 2018**  

(1)	**324k** images with **245** labels that cover 6 categories of women’s clothing, and a total of 41 subcategories (single labeled).  
[[homepage]](https://tianchi.aliyun.com/competition/entrance/231649/information) [[pdf]](http://openaccess.thecvf.com/content_CVPRW_2019/papers/FFSS-USAD/Zou_FashionAI_A_Hierarchical_Dataset_for_Fashion_Understanding_CVPRW_2019_paper.pdf) [[TIANCHI]](https://tianchi.aliyun.com/competition/entrance/231671/introduction?spm=5176.12281949.1003.10.493e1dc1qVUD4c) :pig:

:orange: You may kindly obtain the data by logging in to the TIANCHI platform (Choosing the international version, then register a personal account and sign the agreement. You will be supposed to access the data successfully).
```bib
@inproceedings{zou2019fashionai,
  title={FashionAI: A Hierarchical Dataset for Fashion Understanding},
  author={Zou, Xingxing and Kong, Xiangheng and Wong, Waikeung and Wang, Congde and Liu, Yuguang and Cao, Yang},
  booktitle={Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition Workshops},
  pages={0--0},
  year={2019}
}
```


:cherries: **Feidegger 2018**  

(1) **8,700** fashion items, each with a high-resolution image and **5** independently collected textual descriptions.
(2) Restrict the domain to images of dresses, and German-language visual descriptions.

[[homepage]](https://research.zalando.com/welcome/mission/research-projects/feidegger-dataset/) [[pdf]](http://www.lrec-conf.org/proceedings/lrec2018/pdf/319.pdf)
```bib
@inproceedings{lefakis2018feidegger,
  title={FEIDEGGER: A Multi-modal Corpus of Fashion Images and Descriptions in German},
  author={Lefakis, Leonidas and Akbik, Alan and Vollgraf, Roland},
  booktitle={Proceedings of the Eleventh International Conference on Language Resources and Evaluation (LREC 2018)},
  year={2018}
}
```


:cherries: **Studio2Shop 2018**  

(1) **1.15 million** query images with neutral backgrounds.
(2) Category(7), Color(82), Print(19), Cloth length (12), sleeve length (9), shirt collar(27), Neckline (12), Material (14), Trouser rise (3).

[homepage] [[pdf]](https://www.scitepress.org/Papers/2018/65445/65445.pdf)
```bib
@article{lasserre2018studio2shop,
  title={Studio2shop: from studio photo shoots to fashion articles},
  author={Lasserre, Julia and Rasch, Katharina and Vollgraf, Roland},
  journal={arXiv preprint arXiv:1807.00556},
  year={2018}
}
```


:cherries: **Shopping 100k 2018**  

(1) **101,021** images that consist of pure clothing items.  
(2) Category(16), Neckline(17+11), Color(19), Material(14), Opening(9), Silhouette(15), Gender(2), Cloth length(7), Print(15), Pocket(7), Sleeve length(9), Sport(15).  

[homepage] [[pdf]](https://www.researchgate.net/profile/Kenan_Ak/publication/324728522_Efficient_Multi-Attribute_Similarity_Learning_Towards_Attribute-based_Fashion_Search/links/5adf5078aca272fdaf89c65a/Efficient-Multi-Attribute-Similarity-Learning-Towards-Attribute-based-Fashion-Search.pdf)
```bib
@inproceedings{ak2018efficient,
  title={Efficient multi-attribute similarity learning towards attribute-based fashion search},
  author={Ak, Kenan E and Lim, Joo Hwee and Tham, Jo Yew and Kassim, Ashraf A},
  booktitle={2018 IEEE Winter Conference on Applications of Computer Vision (WACV)},
  pages={1671--1679},
  year={2018},
  organization={IEEE}
}
```


:cherries: **Footwear 2018**  

(1)	**1,000** object, 12 category footwear dataset, each object captured from 4 different poses.  

[[homepage]](https://www.cse.iitd.ac.in/~chetan/projects.html) [[pdf]](https://www.cse.iitd.ac.in/~chetan/papers/icip18-fgvc.pdf)
```bib
@inproceedings{mahajan2018pose,
  title={Pose Aware Fine-Grained Visual Classification Using Pose Experts},
  author={Mahajan, Kushagra and Khurana, Tarasha and Chopra, Ayush and Gupta, Isha and Arora, Chetan and Rai, Atul},
  booktitle={2018 25th IEEE International Conference on Image Processing (ICIP)},
  pages={2381--2385},
  year={2018},
  organization={IEEE}
}
```
:cherries: **iMaterialist 2019**  

(1) **1M+** fashion images with **228** fine-grained attributes in total (multi-labeled).  
(2) Category(105), Color(21), Gender(3), Material(34), Neckline(11), Print(28), Sleeve length(5), Design details(21).  

[[homepage]](https://www.kaggle.com/c/imaterialist-fashion-2019-FGVC6) [[pdf]](http://openaccess.thecvf.com/content_ICCVW_2019/papers/CVFAD/Guo_The_iMaterialist_Fashion_Attribute_Dataset_ICCVW_2019_paper.pdf) [[github]](https://github.com/visipedia/imat_fashion_comp) :pig:
```bib
@inproceedings{guo2019imaterialist,
  title={The imaterialist fashion attribute dataset},
  author={Guo, Sheng and Huang, Weilin and Zhang, Xiao and Srikhanta, Prasanna and Cui, Yin and Li, Yuan and Adam, Hartwig and Scott, Matthew R and Belongie, Serge},
  booktitle={Proceedings of the IEEE International Conference on Computer Vision Workshops},
  pages={0--0},
  year={2019}
}
```


:cherries: **Atlas 2019**  

(1) **186,150** images under clothing category with **3** levels and **52** leaf nodes in the taxonomy.  

[[homepage]](https://github.com/vumaasha/atlas) [[pdf]](https://arxiv.org/pdf/1908.08984.pdf) :pig:
```bib
@article{umaashankar2019atlas,
  title={Atlas: A Dataset and Benchmark for E-commerce Clothing Product Categorization},
  author={Umaashankar, Venkatesh and Prakash, Aditi and others},
  journal={arXiv preprint arXiv:1908.08984},
  year={2019}
}
```


:cherries: **DeepShoe 2019**  

(1) **14,314** and **31,048** images from the street and online shop scenario in multiple viewpoints.  
(2) Attributes including 22 Colors, 4 Toe shape, 7 Heel shape.  

[homepage] [[pdf]](http://alumni.media.mit.edu/~shiboxin/files/Zhan_CVIU19.pdf)
```bib
@article{zhan2019deepshoe,
  title={DeepShoe: An improved Multi-Task View-invariant CNN for street-to-shop shoe retrieval},
  author={Zhan, Huijing and Shi, Boxin and Duan, Ling-Yu and Kot, Alex C},
  journal={Computer Vision and Image Understanding},
  volume={180},
  pages={23--33},
  year={2019},
  publisher={Elsevier}
}
```


:cherries: **FindFashion 2019 combine DeepFashion & Street2Shop**  

(1) Customer-to-shop clothes retrieval dataset consists of **565,041** images and **382,230** pairs.  
(2) Labeled **3** attributes (i.e., occlusions, views, and cropping).  
(3) Divided the benchmark into 4 levels. i.e., Easy, Hard-Cropping, Hard-Occlusion, and Hard-View.  

[homepage] [[pdf]](http://openaccess.thecvf.com/content_ICCV_2019/papers/Kuang_Fashion_Retrieval_via_Graph_Reasoning_Networks_on_a_Similarity_Pyramid_ICCV_2019_paper.pdf) 
```bib
@inproceedings{kuang2019fashion,
  title={Fashion Retrieval via Graph Reasoning Networks on a Similarity Pyramid},
  author={Kuang, Zhanghui and Gao, Yiming and Li, Guanbin and Luo, Ping and Chen, Yimin and Lin, Liang and Zhang, Wayne},
  booktitle={Proceedings of the IEEE International Conference on Computer Vision},
  pages={3066--3075},
  year={2019}
}
```


:cherries: **GarmentSet 2020**  

(1) **9,636** images with collar part annotations and **8,616** images with shoulder and sleeve annotations.  
(2) With annotation of landmarks of collars and sleeves on clean garment images.  

[homepage] [[pdf]](https://arxiv.org/pdf/2001.06427.pdf)
```bib
@inproceedings{chen2020tailorgan,
  title={TailorGAN: Making User-Defined Fashion Designs},
  author={Chen, Lele and Tian, Justin and Li, Guo and Wu, Cheng-Haw and King, Erh-Kan and Chen, Kuan-Ting and Hsieh, Shao-Hang and Xu, Chenliang},
  booktitle={The IEEE Winter Conference on Applications of Computer Vision},
  pages={3241--3250},
  year={2020}
}
```

:cherries: **InFashAIv1 dataset 2021**

(1) contains 15,716 images.  
(2) a large volume of data on African fashion.

[[homepage]](https://github.com/hgilles06/infashai) [[pdf]](https://arxiv.org/pdf/2001.06427.pdf) :pig:
```bib
@inproceedings{chen2020tailorgan,
  title={TailorGAN: Making User-Defined Fashion Designs},
  author={Chen, Lele and Tian, Justin and Li, Guo and Wu, Cheng-Haw and King, Erh-Kan and Chen, Kuan-Ting and Hsieh, Shao-Hang and Xu, Chenliang},
  booktitle={The IEEE Winter Conference on Applications of Computer Vision},
  pages={3241--3250},
  year={2020}
}
```



## 3. &nbsp;Outfit
For outfit generation, recommendation, evaluation, comnpatibility learning *etc*.
******

:cherries: **WoW 2012**  

(1) **24,417** clothing images that are fully annotated.  
(2) **7** multi-value clothing attributes and **10** occasion categories.  
(3) **9,469** images with visible full-body. **8,421** images with only upper-body. **6,527** images with lower-body clothing.  
(4) Color(11), Material(6), Print(6), Neckline(6), Sleeve length(3), Bottom length(3).  
(5) Labeled with **10** common occasions.  

[homepage] [[pdf]](https://dl.acm.org/doi/pdf/10.1145/2393347.2393433)
```bib
@inproceedings{liu2012hi,
  title={Hi, magic closet, tell me what to wear!},
  author={Liu, Si and Feng, Jiashi and Song, Zheng and Zhang, Tianzhu and Lu, Hanqing and Xu, Changsheng and Yan, Shuicheng},
  booktitle={Proceedings of the 20th ACM international conference on Multimedia},
  pages={619--628},
  year={2012}
}
```


:cherries: **Stylatrix**  

[homepage] [[pdf]]  
```bib
@article{sunstylatrix,
  title={Stylatrix: an interactive model-based system for fashion exploration and outfit discovery},
  author={Sun, Will J and Gajos, Krzysztof Z}
}
```


:cherries: **Edge2Garment 2016**  

[[homepage]](https://phillipi.github.io/pix2pix/) [[pdf]](https://arxiv.org/pdf/1810.09941v1.pdf) [[github]](https://github.com/phillipi/pix2pix) [[datalink]](https://people.eecs.berkeley.edu/~tinghuiz/projects/pix2pix/datasets/) :pig:
```bib
@article{pix2pix2016,
  title={Image-to-Image Translation with Conditional Adversarial Networks},
  author={Isola, Phillip and Zhu, Jun-Yan and Zhou, Tinghui and Efros, Alexei A},
  journal={arxiv},
  year={2016}
}
```


:cherries: **FashionVC 2017**  

(1) **20,726** outfits with **14,871** tops and **13,663** bottoms.  
(2) Visual image, categories and title description are collected.  

[homepage] [[pdf]](https://dl.acm.org/doi/pdf/10.1145/3123266.3123314)
```bib
@inproceedings{song2017neurostylist,
  title={Neurostylist: Neural compatibility modeling for clothing matching},
  author={Song, Xuemeng and Feng, Fuli and Liu, Jinhuan and Li, Zekun and Nie, Liqiang and Ma, Jun},
  booktitle={Proceedings of the 25th ACM international conference on Multimedia},
  pages={753--761},
  year={2017}
}
```


:cherries: **Fashion409K 2017**  

(1)	**409,776** sets of clothing items from **644,192** unique items.  

[[homepage]](http://vision.is.tohoku.ac.jp/~tangseng/smart_closet_project.html) [[pdf]](http://openaccess.thecvf.com/content_ICCV_2017_workshops/papers/w32/Tangseng_Recommending_Outfits_From_ICCV_2017_paper.pdf) :pig:
```bib
@InProceedings{Tangseng_2017_ICCV,
author = {Tangseng, Pongsate and Yamaguchi, Kota and Okatani, Takayuki},
title = {Recommending Outfits From Personal Closet},
booktitle = {The IEEE International Conference on Computer Vision (ICCV) Workshops},
month = {Oct},
year = {2017}
}
```


:cherries: **Polyvore 2017**  

(1)  **21,889** outfits and **164,379** items.  
(2) Keep the first **8** for simplicity, the average number of fashion items in an outfit is **6.5**.  
(3) To clean the text descriptions, words appearing fewer than 30 times are deleted, leading to a vocabulary of size **2,757**.  

[homepage] [[pdf]](https://arxiv.org/pdf/1707.05691.pdf) [[github]](https://github.com/xthan/polyvore) :pig:
```bib
@inproceedings{han2017learning,
  author = {Han, Xintong and Wu, Zuxuan and Jiang, Yu-Gang and Davis, Larry S},
  title = {Learning Fashion Compatibility with Bidirectional LSTMs},
  booktitle = {ACM Multimedia},
  year  = {2017},
}
```


:cherries: **AVA 2017**  

(1) Photo.net dataset contains **20,278** images with at least 10 score ratings per image.  
(2) CUHK-PhotoQuality (CUHK-PQ) dataset t contains **17,690** images. All images are given a binary aesthetic label.  
(3)	Aesthetic Visual Analysis (AVA) dataset contains **250k** images. Each image receives 78 ∼ 549 votes of score ranging from 1 to 10.  

[[homepage]](http://personal.ie.cuhk.edu.hk/~dy015/ImageAesthetics/Image_Aesthetic_Assessment.html) [[pdf]](https://arxiv.org/pdf/1610.00838.pdf) :pig:
```bib
@article{deng2017image,
 author = {Deng, Yubin and Loy, Chen Change and Tang, Xiaoou},
 title = {Image Aesthetic Assessment: An Experimental Survey},
 journal={IEEE Signal Processing Magazine},
 volume={34},
 number={4},
 pages={80--106},
 year={2017},
 publisher={IEEE}
}
```


:cherries: **UIUC 2018**  

(1) **68,306** outfits and **365,054** items.  
(2) **19** max items, which has semantic category labeled.  

[homepage] [[pdf]](http://openaccess.thecvf.com/content_ECCV_2018/papers/Mariya_Vasileva_Learning_Type-Aware_Embeddings_ECCV_2018_paper.pdf) [[github]](https://github.com/mvasil/fashion-compatibility) 
```bib
@inproceedings{VasilevaECCV18FasionCompatibility,
Author = {Mariya I. Vasileva and Bryan A. Plummer and Krishna Dusad and Shreya Rajpal and Ranjitha Kumar and David Forsyth},
Title = {Learning Type-Aware Embeddings for Fashion Compatibility},
booktitle = {ECCV},
Year = {2018}
}
```


:cherries: **IQON 2018**  

(1)	**164,837** items of clothing grouped in **21,889** outfits.  

[homepage] [[pdf]](https://arxiv.org/pdf/1807.03133.pdf) [[github]](https://github.com/Cherrybruin/iqon-dataset)
```bib
@article{nakamura2018outfit,
  title={Outfit generation and style extraction via bidirectional lstm and autoencoder},
  author={Nakamura, Takuma and Goto, Ryosuke},
  journal={arXiv preprint arXiv:1807.03133},
  year={2018}
}
```


:cherries: **Style4BodyShape 2018**  

(1)	**3,150** female celebrities annotated with the corresponding types of body shapes.  
(2) **349,298** images of **270** stylish celebrities annotated with the types of clothing items.  

[homepage] [[pdf]](https://dl.acm.org/doi/pdf/10.1145/3240508.3240546)
```bib
@inproceedings{hidayati2018dress,
  title={What dress fits me best? fashion recommendation on the clothing style for personal body shape},
  author={Hidayati, Shintami Chusnul and Hsu, Cheng-Chun and Chang, Yu-Ting and Hua, Kai-Lung and Fu, Jianlong and Cheng, Wen-Huang},
  booktitle={Proceedings of the 26th ACM international conference on Multimedia},
  pages={438--446},
  year={2018}
}
```


:cherries: **Lookastic 2019**  

(1) **30,790** fashionable outfits from the Lookastic.  
(2) **124,665** matched pairs for men with **5,069** items.  
(3) **158,755** matched pairs for women with **10,016** items.  
(4) 65 Colors, 38 Materials, 40 Print, 253 fine-grained Categories, 11 Styles, and 114 Sub-categories.  

[homepage] [[pdf]](http://staff.ustc.edu.cn/~hexn/papers/sigir19-fashion.pdf)
```bib
@inproceedings{yang2019interpretable,
  title={Interpretable Fashion Matching with Rich Attributes},
  author={Yang, Xun and He, Xiangnan and Wang, Xiang and Ma, Yunshan and Feng, Fuli and Wang, Meng and Chua, Tat-Seng},
  booktitle={Proceedings of the 42nd International ACM SIGIR Conference on Research and Development in Information Retrieval},
  pages={775--784},
  year={2019}
}
```


:cherries: **POG 2019**  

(1) **1.01 million** outfits, **583K** fashion items, with context information.  
(2) **0.28 billion** user click actions from **3.57 million** users.  

[homepage] [[pdf]](https://arxiv.org/pdf/1905.01866.pdf) [[github]](https://github.com/wenyuer/POG) :pig:
```bib
@inproceedings{chen2019pog,
  title={POG: Personalized Outfit Generation for Fashion Recommendation at Alibaba iFashion},
  author={Chen, Wen and Huang, Pipei and Xu, Jiaming and Guo, Xin and Guo, Cheng and Sun, Fei and Li, Chao and Pfadler, Andreas and Zhao, Huan and Zhao, Binqiang},
  booktitle={Proceedings of the 25th ACM SIGKDD International Conference on Knowledge Discovery \& Data Mining},
  pages={2662--2670},
  year={2019}
}
```


:cherries: **Shop the Look 2019**  

(1) Based on Shop the Look (STL) task, and covert STL data into a format that can be used for our Complete the Look (CTL) task.  

[homepage] [[pdf]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Kang_Complete_the_Look_Scene-Based_Complementary_Product_Recommendation_CVPR_2019_paper.pdf)[[github]](https://github.com/kang205/STL-Dataset) 
```bib
@inproceedings{kang2019complete,
  title={Complete the Look: Scene-based Complementary Product Recommendation},
  author={Kang, Wang-Cheng and Kim, Eric and Leskovec, Jure and Rosenberg, Charles and McAuley, Julian},
  booktitle={Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition},
  pages={10532--10541},
  year={2019}
}
```


:cherries: **ExpFashion 2019**  

(1) FashionVC+, consisting of both the visual and textual metadata of fashion items (i.e.,the tops, bottoms and shoes) on Polyvore.  
(2) **20,726** outfits with **14,870** tops, **13,662** bottoms and **14,093** pairs of shoes, respectively.  
(3) ExpFashion dataset consists of **893,991** outfits with **168,682** tops and **117,668** bottom.  

[homepage] [[pdf]](https://xuemengsong.github.io/Neuro_2019.pdf)
```bib
@article{liu2019neural,
  title={Neural fashion experts: I know how to make the complementary clothing matching},
  author={Liu, Jinhuan and Song, Xuemeng and Chen, Zhumin and Ma, Jun},
  journal={Neurocomputing},
  volume={359},
  pages={249--263},
  year={2019},
  publisher={Elsevier}
}
```


:cherries: **ASOS outfits 2019**  

(1) **586,320** fashion outfits (images and textual descriptions) composed by ASOS stylists.  
(2) Each containing between 2 and 5 items.  
(3) **591,725** unique items representing **18** different womenswear product types and **22** different menswear product type.  

[homepage] [[pdf]](https://arxiv.org/pdf/1904.00741.pdf)
```bib
@article{bettaney2019fashion,
  title={Fashion Outfit Generation for E-commerce},
  author={Bettaney, Elaine M and Hardwick, Stephen R and Zisimopoulos, Odysseas and Chamberlain, Benjamin Paul},
  journal={arXiv preprint arXiv:1904.00741},
  year={2019}
}
```


:cherries: **Chuanda 2020**  

(1) **3,557** outfits covering **67** basic fashion styles.  
(2) Labeled with **1,879** distinct fashion related attributes that belong to 5 types: Gender, Season, Style, Material, and Function.  

[homepage] [[pdf]](https://arxiv.org/pdf/2004.06229.pdf)
```bib
@article{liu2020imitation,
  title={Imitation Learning for Fashion Style Based on Hierarchical Multimodal Representation},
  author={Liu, Shizhu and Yang, Shanglin and Zhou, Hui},
  journal={arXiv preprint arXiv:2004.06229},
  year={2020}
}
```


## 4. &nbsp;Generation
For 3D generation, VTON *etc*.
*******

:cherries: **MPI Dynamic FAUST | BUFF 2017**  

(1)	**40,000** raw and aligned meshes.  

[[homepage]](http://buff.is.tue.mpg.de/) [[pdf]](http://openaccess.thecvf.com/content_cvpr_2017/papers/Bogo_Dynamic_FAUST_Registering_CVPR_2017_paper.pdf) :pig:
```bib
@inproceedings{dfaust:CVPR:2017,
  title = {Dynamic {FAUST}: {R}egistering Human Bodies in Motion},
  author = {Bogo, Federica and Romero, Javier and Pons-Moll, Gerard and Black, Michael J.},
  booktitle = {IEEE Conf. on Computer Vision and Pattern Recognition (CVPR)},
  month = jul,
  year = {2017},
  month_numeric = {7}
}
```


:cherries: **FashionGAN 2017** 

(1)	Extended the DeepFashion by collecting sentence descriptions for **79K** images.  

[homepage] [[pdf]](http://openaccess.thecvf.com/content_ICCV_2017/papers/Zhu_Be_Your_Own_ICCV_2017_paper.pdf) [[github]](https://github.com/zhusz/ICCV17-fashionGAN) :pig:
```bib
@inproceedings{zhu2017be,
  title={Be Your Own Prada: Fashion Synthesis with Structural Coherence},
  author={Zhu, Shizhan and Fidler, Sanja and Urtasun, Raquel and Lin, Dahua and Chen, Change Loy},
  booktitle={Proceedings of the IEEE Conference on International Conference on Computer Vision},
  year={2017}
}
```


:cherries: **BeautyGAN 2018**  

(1)	Facial makeup dataset consists of **3,834** female images.  

[[homepage]](http://liusi-group.com/projects/BeautyGAN) [[pdf]](https://dl.acm.org/doi/pdf/10.1145/3240508.3240618) :pig:
```bib
@inproceedings{li2018beautygan,
  title={Beautygan: Instance-level facial makeup transfer with deep generative adversarial network},
  author={Li, Tingting and Qian, Ruihe and Dong, Chao and Liu, Si and Yan, Qiong and Zhu, Wenwu and Lin, Liang},
  booktitle={Proceedings of the 26th ACM international conference on Multimedia},
  pages={645--653},
  year={2018}
}
```


:cherries: **VTON 2018**  

(1)	Collected dataset from Zalando.  
(2)	**19,000** frontal-view woman and top2 image pairs (removed noisy images with no parsing results), yielding **16,253** pairs.  

[homepage] [[pdf]](http://openaccess.thecvf.com/content_cvpr_2018/papers/Han_VITON_An_Image-Based_CVPR_2018_paper.pdf) [[github]](https://github.com/xthan/VITON) 
```bib
@inproceedings{han2017viton,
  title = {VITON: An Image-based Virtual Try-on Network},
  author = {Han, Xintong and Wu, Zuxuan and Wu, Zhe and Yu, Ruichi and Davis, Larry S},
  booktitle = {CVPR},
  year  = {2018},
}
```


:cherries: **DeepWear 2018**  

(1)	A specific brand clothes dataset.  

[homepage] [[pdf]](https://digitalnature.slis.tsukuba.ac.jp/wp-content/uploads/2018/03/deepwear.pdf)
```bib
@inproceedings{kato2018deepwear,
  title={DeepWear: a Case Study of Collaborative Design between Human and Artificial Intelligence},
  author={Kato, Natsumi and Osone, Hiroyuki and Sato, Daitetsu and Muramatsu, Naoya and Ochiai, Yoichi},
  booktitle={Proceedings of the Twelfth International Conference on Tangible, Embedded, and Embodied Interaction},
  pages={529--536},
  year={2018}
}
```


:cherries: **FashionGEN 2018**  

(1)	**293,008** high-resolution fashion images paired with item descriptions provided by professional stylists.  
(2)	All fashion items are photographed from 1 to 6 different angles depending on the category of the item.  
(3)	**48** main categories, and **121** fine-grained sub-categories.  
(4)	Paired with paragraph-length descriptive captions sourced from experts (professional designers).  
(5)	Provide metadata such as stylist recommended matched items, the fashion season, designer and the brand.  
(6)	Provide the distribution of colors extracted from the text description.  

[[homepage]](https://fashion-gen.com/) [[pdf]](https://arxiv.org/pdf/1806.08317.pdf)
```bib
@article{rostamzadeh2018fashion,
  title={Fashion-gen: The generative fashion dataset and challenge},
  author={Rostamzadeh, Negar and Hosseini, Seyedarian and Boquet, Thomas and Stokowiec, Wojciech and Zhang, Ying and Jauvin, Christian and Pal, Chris},
  journal={arXiv preprint arXiv:1806.08317},
  year={2018}
}
```


:cherries: **ZalandoGAN 2018**  

(1)	Over **120,000** images of dresses that are downloaded from Zalando’s website.  

[[homepage]](https://research.zalando.com/welcome/mission/research-projects/generative-fashion-design/) [[pdf]](https://arxiv.org/pdf/1806.07819.pdf) [[github]](https://github.com/zalandoresearch/disentangling_conditional_gans)
```bib
@article{yildirim2018disentangling,
  title={Disentangling multiple conditional inputs in gans},
  author={Yildirim, G{\"o}khan and Seward, Calvin and Bergmann, Urs},
  journal={arXiv preprint arXiv:1806.07819},
  year={2018}
}
```


:cherries: **RTW 2018**  

(1)	Augment the dataset of **4,157** images by a factor 5 by jittering images with random scaling and translations.  
(2)	7 categories: jackets, coats, shirts, tops, t-shirts, dresses and pullovers.  
(3)	7 print: plain(uniform), plain(tiled?), striped, animal print(animal skin), dotted, graphic print(print and graphical pattern).  

[homepage] [[pdf]](http://openaccess.thecvf.com/content_ECCVW_2018/papers/11131/Sbai_DesIGN_Design_Inspiration_from_Generative_Networks_ECCVW_2018_paper.pdf)
```bib
@inproceedings{sbai2018design,
  title={Design: Design inspiration from generative networks},
  author={Sbai, Othman and Elhoseiny, Mohamed and Bordes, Antoine and LeCun, Yann and Couprie, Camille},
  booktitle={Proceedings of the European Conference on Computer Vision (ECCV)},
  pages={0--0},
  year={2018}
}
```


:cherries: **SMPL 2018**  

(1)	Comprises a pair of jeans, a T-shirt and a sweater worn by **600** bodies in various poses.  

[[homepage]](https://www.epfl.ch/labs/cvlab/research/garment-simulation/garnet/) [[pdf]](http://openaccess.thecvf.com/content_ICCV_2019/papers/Gundogdu_GarNet_A_Two-Stream_Network_for_Fast_and_Accurate_3D_Cloth_ICCV_2019_paper.pdf) 
```bib
@inproceedings{gundogdu19garnet,
title = {Garnet: A Two-stream Network for Fast and Accurate 3D Cloth Draping},
author = {Gundogdu, Erhan and Constantin, Victor and Seifoddini, Amrollah and Dang, Minh and Salzmann, Mathieu and Fua, Pascal},
booktitle = {{IEEE} International Conference on Computer Vision ({ICCV})},
month = {oct},
organization = {{IEEE}},
year = {2019},
}
```

:cherries: **MVP 2019**  

(1)	Contains **35,687** person images and **13,524** clothes images.
(2) Each person image in MPV has different poses.
(3) The image is in the resolution of 256 × 192.
(4) 62,780 three-tuples of the same person in the same clothes but with different poses.

[[homepage]](https://github.com/thaithanhtuan/MyMGVTON) [[pdf]](http://openaccess.thecvf.com/content_ICCV_2019/papers/Dong_Towards_Multi-Pose_Guided_Virtual_Try-On_Network_ICCV_2019_paper.pdf) :pig:
```bib
@inproceedings{dong2019towards,
  title={Towards multi-pose guided virtual try-on network},
  author={Dong, Haoye and Liang, Xiaodan and Shen, Xiaohui and Wang, Bochao and Lai, Hanjiang and Zhu, Jia and Hu, Zhiting and Yin, Jian},
  booktitle={Proceedings of the IEEE International Conference on Computer Vision},
  pages={9026--9035},
  year={2019}
}
```

:cherries: **AMASS dataset 2019** 

AMASS is a large database of human motion unifying different optical marker-based motion capture datasets by representing them within a common framework and parameterization. AMASS is readily useful for animation, visualization, and generating training data for deep learning.

(1) more than 40 hours of motion data, spanning over 300 subjects, more than 11000 motions

[[homepage]](https://amass.is.tue.mpg.de/)[[pdf]](https://arxiv.org/pdf/1904.03278.pdf)
```bib
@inproceedings{AMASS:2019,
  title={AMASS: Archive of Motion Capture as Surface Shapes},
  author={Mahmood, Naureen and Ghorbani, Nima and F. Troje, Nikolaus and Pons-Moll, Gerard and Black, Michael J.},
  booktitle = {The IEEE International Conference on Computer Vision (ICCV)},
  year={2019},
  month = {Oct},
  url = {https://amass.is.tue.mpg.de},
  month_numeric = {10}
}
```



:cherries: **Fashion Takes 2019**  

(1)	Over **18,000** images with meta-data including clothing category.  
(2)	Manual shape annotation indicating whether the person’s shape is above average or average.  
(3)	The data comprises 181 different users.  
(4) Allowed to study ** the relationship between clothing categories and body shape**.  

[homepage] [[pdf]](https://virtualhumans.mpi-inf.mpg.de/papers/sattar2019WACV/sattar2019WACV.pdf)
```bib
@inproceedings{sattar2019fashion,
  title={Fashion is taking shape: Understanding clothing preference based on body shape from online sources},
  author={Sattar, Hosnieh and Pons-Moll, Gerard and Fritz, Mario},
  booktitle={2019 IEEE Winter Conference on Applications of Computer Vision (WACV)},
  pages={968--977},
  year={2019},
  organization={IEEE}
}
```


:cherries: **StyleGAN 2019**  

(1) Based on a proprietary image dataset with around **380k** entries with high-resolution.  
(2) An outfit is composed of a set of the maximum of **6** articles.  

[homepage] [[pdf]](http://openaccess.thecvf.com/content_ICCVW_2019/papers/CVFAD/Yildirim_Generating_High-Resolution_Fashion_Model_Images_Wearing_Custom_Outfits_ICCVW_2019_paper.pdf)
```bib
@inproceedings{yildirim2019generating,
  title={Generating High-Resolution Fashion Model Images Wearing Custom Outfits},
  author={Yildirim, Gokhan and Jetchev, Nikolay and Vollgraf, Roland and Bergmann, Urs},
  booktitle={Proceedings of the IEEE International Conference on Computer Vision Workshops},
  pages={0--0},
  year={2019}
}
```


:cherries: **Deep Fashion3D 2020**  

(1)	**2,078** models reconstructed from real garments, which covers **10** different categories and **563** garment instances.  
(2)	Multi-view stereo, multi-view real images, 3D feature lines, 3D body pose.  

[[homepage]](https://kv2000.github.io/2020/03/25/deepFashion3DRevisited/) [[pdf]](https://arxiv.org/pdf/2003.12753.pdf) :pig:
```bib
@article{zhu2020deep,
  title={Deep Fashion3D: A Dataset and Benchmark for 3D Garment Reconstruction from Single Images},
  author={Zhu, Heming and Cao, Yu and Jin, Hang and Chen, Weikai and Du, Dong and Wang, Zhangye and Cui, Shuguang and Han, Xiaoguang},
  journal={arXiv preprint arXiv:2003.12753},
  year={2020}
}
```

:cherries: **CAPE 2020**

(1) provides SMPL mesh registration of 4D scans of people in clothing, along with registered scans of the ground truth body shapes under clothing. 
(2) 10 male and 5 female subjects.
(3) 600+ motion sequences, 140K+ frames, 4 different types of outfits: short upper body clothing with long trousers (denoted as "short long"), and "short short", "long short", "long long"
(4) covers 8 common garment types: short T-shirts, long T-shirts, long jerseys, long-sleeve shirts, polo shirts, blazers, shorts, long trousers.

[[homepage]](https://cape.is.tue.mpg.de/dataset.html) [[pdf]](https://arxiv.org/pdf/1907.13615.pdf) :pig:
```bib
@inproceedings{CAPE:CVPR:20,
  title = {{Learning to Dress 3D People in Generative Clothing}},
  author = {Ma, Qianli and Yang, Jinlong and Ranjan, Anurag and Pujades, Sergi and Pons-Moll, Gerard and Tang, Siyu and Black, Michael J.},
  booktitle = {Computer Vision and Pattern Recognition (CVPR)},
  month = June,
  year = {2020},
  month_numeric = {6}}
```

:cherries: **CLOTH3D 2021**

(1) consisting of 2, 300 3D point cloud sequences by adapting CLOTH3D, which serves as the first benchmark dataset for evaluating posed garment reconstruction based on point cloud sequences.

[[homepage]](https://hongfz16.github.io/projects/Garment4D.html) [[pdf]](https://papers.nips.cc/paper/2021/file/eb160de1de89d9058fcb0b968dbbbd68-Paper.pdf) :pig:
```bib
@inproceedings{
    hong2021garmentd,
    title={Garment4D: Garment Reconstruction from Point Cloud Sequences},
    author={Fangzhou Hong and Liang Pan and Zhongang Cai and Ziwei Liu},
    booktitle={Thirty-Fifth Conference on Neural Information Processing Systems},
    year={2021},
    url={https://openreview.net/forum?id=aF60hOEwHP}
}
```


:cherries: **AGORA 2021**

(1) 4240 commercially available, high-quality, textured human scans in diverse poses and natural clothing; this includes 257 scans of children. We create reference 3D poses and body shapes by fitting the SMPL-X body model (with face and hands) to the 3D scans, taking into account clothing. 
(2) around 14K training and 3K test images by rendering between 5 and 15 people per image using either image-based lighting or rendered 3D environments, taking care to make the images physically plausible and photoreal. 
(3) consists of 173K individual person crops.

[[homepage]](https://agora.is.tue.mpg.de/) [[pdf]](https://arxiv.org/pdf/2104.14643.pdf) :pig:
```bib
@inproceedings{Patel:CVPR:2021,
  title = {{AGORA}: Avatars in Geography Optimized for Regression Analysis}, 
  author = {Patel, Priyanka and Huang, Chun-Hao P. and Tesch, Joachim and Hoffmann, David T. and Tripathi, Shashank and Black, Michael J.}, 
  booktitle = {Proceedings IEEE/CVF Conf.~on Computer Vision and Pattern Recognition ({CVPR})}, 
  month = jun,
  year = {2021},
  month_numeric = {6}
}
```

:cherries: **ReSynth Dataset 2021**

(1) contains 24 outfits of diverse garment types, dressed on varied body shapes across both genders, as shown in the image below.
(2) the clothing designs are created by a professional clothing designer so that they faithfully reflect those in the real scanned human dataset (RenderPeople).
(3) all outfits are simulated using a consistent set of 20 motion sequences captured in the CAPE dataset.

[[homepage]](https://pop.is.tue.mpg.de/) [[pdf]](https://arxiv.org/pdf/2109.01137.pdf) :pig:
```bib
@inproceedings{POP:ICCV:2021,
title = {The Power of Points for Modeling Humans in Clothing},
author = {Ma, Qianli and Yang, Jinlong and Tang, Siyu and Black, Michael J.},
booktitle = {Proceedings of the IEEE/CVF International Conference on Computer Vision (ICCV)},
month = oct,
year = {2021},
month_numeric = {10}}
```

## 5. &nbsp;Others
:cherries: **Amazon Reviews 2015**  

(1) Based on the **Amazon** web store.  
(2) Over **180 million** relationships between a pool of almost 6 million objects.  

[[homepage]](https://nijianmo.github.io/amazon/index.html) [[pdf]](https://dl.acm.org/doi/pdf/10.1145/2766462.2767755)
```bib
@inproceedings{mcauley2015image,
  title={Image-based recommendations on styles and substitutes},
  author={McAuley, Julian and Targett, Christopher and Shi, Qinfeng and Van Den Hengel, Anton},
  booktitle={Proceedings of the 38th International ACM SIGIR Conference on Research and Development in Information Retrieval},
  pages={43--52},
  year={2015}
}
```


:cherries: **Tradesy 2016**  

(1)	**19,823** users, **166,526** items, **410,186** feedback.  
(2)	Contains users’ purchase histories and ‘thumbs-up’.  

[[homepage]](http://jmcauley.ucsd.edu/data/tradesy/) [[pdf]](http://cseweb.ucsd.edu/~jmcauley/pdfs/aaai16.pdf) :pig:
```bib
@inproceedings{he2016vbpr,
  title={VBPR: visual bayesian personalized ranking from implicit feedback},
  author={He, Ruining and McAuley, Julian},
  booktitle={Thirtieth AAAI Conference on Artificial Intelligence},
  year={2016}
}
```


:cherries: **Fashion-MNIST 2017**  

(1)	Comprising of 28 × 28 grayscale images of **70,000** fashion products from 10 categories.  

[[homepage]](https://research.zalando.com/welcome/mission/research-projects/fashion-mnist/) [[pdf]](https://arxiv.org/pdf/1708.07747.pdf) [[github]](https://github.com/zalandoresearch/fashion-mnist) :pig:
```bib
@online{xiao2017/online,
  author       = {Han Xiao and Kashif Rasul and Roland Vollgraf},
  title        = {Fashion-MNIST: a Novel Image Dataset for Benchmarking Machine Learning Algorithms},
  date         = {2017-08-28},
  year         = {2017},
  eprintclass  = {cs.LG},
  eprinttype   = {arXiv},
  eprint       = {cs.LG/1708.07747},
}
```


:cherries: **Shoe 2018**  

(1)	Supports further research on the task of relative **image captioning**.  
(2)	Pairing **3,600** captions that were discriminative with additional dissimilar images.  

[homepage] [[pdf]](http://papers.nips.cc/paper/7348-dialog-based-interactive-image-retrieval.pdf)
```bib
@inproceedings{guo2018dialog,
  title={Dialog-based interactive image retrieval},
  author={Guo, Xiaoxiao and Wu, Hui and Cheng, Yu and Rennie, Steven and Tesauro, Gerald and Feris, Rogerio},
  booktitle={Advances in Neural Information Processing Systems},
  pages={678--688},
  year={2018}
}
```


:cherries: **Flickr30k 2018**  

(1)	**300k** posts with **5M** comments.  
(2)	Each image is paired with user comment. The maximum number of comments is 427, average per image is 14.  

[homepage] [[pdf]](https://dl.acm.org/doi/pdf/10.1145/3184558.3186354)
```bib
@inproceedings{lin2018netizen,
  title={Netizen-style commenting on fashion photos: dataset and diversity measures},
  author={Lin, Wen Hua and Chen, Kuan-Ting and Chiang, Hung Yueh and Hsu, Winston},
  booktitle={Companion Proceedings of the The Web Conference 2018},
  pages={395--402},
  year={2018}
}
```
:cherries: **FCDB 2019**  

(1)	**100 million** Flickr images which focus on 21 global cities based on city perception.  
(2)	**25,707,690** clothing images for **trend analysis**.  

[[homepage]](http://hirokatsukataoka.net/) [[pdf]](http://openaccess.thecvf.com/content_CVPRW_2019/papers/FFSS-USAD/Kataoka_Ten-Million-Order_Human_Database_for_World-Wide_Fashion_Culture_Analysis_CVPRW_2019_paper.pdf) [[github]](https://github.com/cvpaperchallenge/FashionCultureDataBase_DLoader) :pig:
```bib
@InProceedings{Kataoka_2019_CVPR_Workshops,
author = {Kataoka, Hirokatsu and Satoh, Yutaka and Abe, Kaori and Minoguchi, Munetaka and Nakamura, Akio},
title = {Ten-Million-Order Human Database for World-Wide Fashion Culture Analysis},
booktitle = {The IEEE Conference on Computer Vision and Pattern Recognition (CVPR) Workshops},
month = {June},
year = {2019}
}
```


:cherries: **Fashion IQ 2019**  

(1)	Dataset for **natural language based fashion image retrieval**.  
(2)	Each image is crawled from Amazon.com and extracted corresponding product information, when available.  

[homepage] [[pdf]](https://arxiv.org/pdf/1905.12794.pdf) [[github]](https://github.com/XiaoxiaoGuo/fashion-iq) [[github]](https://github.com/XiaoxiaoGuo/fashion-iq) :pig:
```bib
@article{guo2019fashion,
  title={The Fashion IQ Dataset: Retrieving Images by Combining Side Information and Relative Natural Language Feedback},
  author={Guo, Xiaoxiao and Wu, Hui and Gao, Yupeng and Rennie, Steven and Feris, Rogerio},
  journal={arXiv preprint arXiv:1905.12794},
  year={2019}
}
```


:cherries: **TFCD 2019**  

(1)	A dataset containing data from real user sessions on a major European e-commerce fashion website.  

[homepage] [[pdf]](https://arxiv.org/ftp/arxiv/papers/1907/1907.00400.pdf)
```bib
@article{bigon2019prediction,
  title={Prediction is very hard, especially about conversion. Predicting user purchases from clickstream data in fashion e-commerce},
  author={Bigon, Luca and Cassani, Giovanni and Greco, Ciro and Lacasa, Lucas and Pavoni, Mattia and Polonioli, Andrea and Tagliabue, Jacopo},
  journal={arXiv preprint arXiv:1907.00400},
  year={2019}
}
```

:cherries: **SHIFT15M 2021**

(1) a dataset that can be used to properly evaluate models in situations where the distribution of data changes between training and testing.
(2) Multiobjective, each instance in the dataset has several numerical values that can be used as target variables. 
(3) Large-scale, the SHIFT15M dataset consists of 15million fashion images. 
(4) Coverage of types of dataset shifts. It contains multiple dataset shift problem settings.

[[homepage]](https://github.com/st-tech/zozo-shift15m) [[pdf]](https://arxiv.org/pdf/2108.12992.pdf) :pig:
```bib
@article{kimura2021shift15m,
  title={SHIFT15M: Multiobjective Large-Scale Fashion Dataset with Distributional Shifts},
  author={Kimura, Masanari and Nakamura, Takuma and Saito, Yuki},
  journal={arXiv preprint arXiv:2108.12992},
  year={2021}
}
```

:cherries: **3D Garments with Sewing Patterns 2021**

(1) consisting of 19 garment types and more then 20 000 garment samples.

[[homepage]](https://github.com/maria-korosteleva/Garment-Pattern-Generator) [[pdf]](https://arxiv.org/pdf/2109.05633.pdf) :pig:
```bib
@article{korosteleva2021generating,
  title={Generating Datasets of 3D Garments with Sewing Patterns},
  author={Korosteleva, Maria and Lee, Sung-Hee},
  year={2021}
}
```

## Other Sources
- MPV (Multi-Pose Virtual try on) dataset [[link]](http://sysu-hcp.net/lip/overview.php)
- Clothing Attributes Dataset [[link]](https://exhibits.stanford.edu/data/catalog/tb980qz1002)
- Clothing Detection Dataset [[link]](https://github.com/seralexger/clothing-detection-dataset)
- Clothing Size Recommendation [[link]](https://github.com/NeverInAsh/fit-recommendation)
- Fashion Product Image [[link]](https://www.kaggle.com/paramaggarwal/fashion-product-images-dataset)
- Dresses_Attribute_Sales Data Set [[link]](https://archive.ics.uci.edu/ml/datasets/Dresses_Attribute_Sales)
- HICP-Clothing [[link]](https://data.europa.eu/euodp/en/data/dataset/sE1cgO8hyGVp2RxD9iafA)
- Paper Doll Raw Dataset [[link]](https://github.com/kyamagu/paperdoll/tree/master/data/chictopia)
- Fashion Toolbox [[link]](https://github.com/open-mmlab/mmfashion)
- https://data.world/datasets/fashion
- https://tianchi.aliyun.com/dataset/
## Acknowledge
Here I would like to thank Miss Po Yee(Boey), PANG, Miss Wai Lee(Selene), CHONG, for their hard work on collecting the datasource information.
