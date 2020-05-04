# DATASOURCE for *fAshIon* :thought_balloon:

This is a summary. We reviewed all  (to our best knowledge) fashion-related papers in the past decade and recorded the datasets been used. The numbers to describe the dataset is faithfully followed its original paper.  

:pig: means the dataset can be found  

We uniformed the words decribe the fashion concept.
- &nbsp;**Silhouette** (shape): the shape of a garment, *e.g.* H line, A line *etc*;
- &nbsp;**Material** (fabric): the material made a garment, *e.g.* chiffon, lace *etc*;
- &nbsp;**Print** (pattern): the surface design of a garment, *e.g.* checks, dotted *etc*;
- &nbsp;**Neckline** (collar shape)： the design in the neck region of a garment， *e.g.* V-neck, lapel *etc*; 
- &nbsp;**Category** (type): type of a garment, *e.g.* dress, top *etc*;
- &nbsp;**Sub-category**: fine-grained type of a garment, *e.g.* wedding dress, T-shire *etc*;
- &nbsp;**Style**: the expressed feeling of a garment of an outfit, *e.g.* lovely, casual *etc*;
- &nbsp;**Design Attributes**: the attributes used in the process of garment design, *e.g.* shirt cuff, shirt collar *etc*;
- &nbsp;**Retail Attributes**: the attributes used in the process of retail, *e.g.*  parka, windbreaker *etc*.  

If you have problems with a specific dataset shows below, please kindly contact its authors. For quick check, you can also see [memo version](https://drive.google.com/open?id=1ucwMgee0Df1P--cDHQR9XdcPPuMjgaSt) &copy;

## 0. &nbsp;Parsing 
For semantic segmentation, object detection, instance segmentation, polygon detection, and *etc*.
*****
`#f03c15`**Fashionista 2012** :pig:  

(1) **158,235** fashion photos with associated text annotations (tags, comments, and links).  
(2) The tags are noisy or incomplete.  
(3) **685** photos with good visibility of the full-body with pose annotations for the usual 14 body parts.  
(4) There are totally **56** labels (**53** category or sub-category labels, and additional labels for hair, skin, and null (background).  

[[homepage]](http://vision.is.tohoku.ac.jp/~kyamagu/research/clothing_parsing/) [[pdf]](http://vision.is.tohoku.ac.jp/~kyamagu/papers/yamaguchi_cvpr2012.pdf) 
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
  
**Paperdoll 2013** :pig:  

(1) Over **1 million** pictures from chictopia.com with associated metadata tags i.e. color, clothing item, or occasion.  
(2) **339,797** pictures weakly annotated with clothing items and estimated pose.  
(3) **685** fully parsed images .

[[homepage]](http://vision.is.tohoku.ac.jp/~kyamagu/research/paperdoll/) [[pdf]](https://www.cv-foundation.org/openaccess/content_iccv_2013/papers/Yamaguchi_Paper_Doll_Parsing_2013_ICCV_paper.pdf) 
```bib
@inproceedings{yamaguchi2013paper,
  title={Paper doll parsing: Retrieving similar styles to parse clothing items},
  author={Yamaguchi, Kota and Hadi Kiapour, M and Berg, Tamara L},
  booktitle={Proceedings of the IEEE international conference on computer vision},
  pages={3519--3526},
  year={2013}
}
```

**CFPD 2013** :pig:  

(1) **97,490** images with 292,541 tags from Chictopia.com.  
(2) **2,682** images in total, and all the pixels in the images are annotated with both color labels (**13**) and category labels (**23**).   
(3) **Weakly supervised setting**, where only image-level tags are available in the training phase.

[[pdf]](https://liusi-group.com/pdf/Fashion%20Parsing%20With%20Weak%20Color-Category%20Labels.pdf) [[github1]](https://github.com/zbxzc35/dataset-CFPD) [[github2]](https://github.com/hrsma2i/dataset-CFPD) 
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
**CCP 2013** :pig:    

(1) It consisting of **2098** high-resolution street fashion photos.  
(2) More than **1,000** images are annotated with superpixel-level labeling with a total of **57** tags.  
(3) Cross-scenario image pairs, which include about **10,000** product photos and user's photos image pairs.   
(4) Each image has **124** fine-grained semantic attributes.  
(5) **20** categories, **56** colors, **6** clothing length, **10** silhouette, **25** necklines, and **7** sleeve length. 
 
[[homepage]](http://www.sysu-hcp.net/clothing-co-parsing-by-joint-image-segmentation-and-labeling/) [[pdf]](http://linliang.net/wp-content/uploads/2017/07/TMM_Clothes.pdf) [[github]](https://github.com/bearpaw/clothing-co-parsing) 
```bib
@inproceedings{yang2014clothing,
  title={Clothing Co-Parsing by Joint Image Segmentation and Labeling},
  author={Yang, Wei and Luo, Ping and Lin, Liang}
  booktitle={Computer Vision and Pattern Recognition (CVPR), 2014 IEEE Conference on},
  year={2013},
  organization={IEEE}
}
```
**HCP 2015** :pig:  

(1) **7,700** images in total.  
(2) Combined Fashionista (685), CFPD (2,682), Daily Photos dataset (2,500).  
(3) Crawl another **1,833** challenging images （*e.g.* sitting or occlusion) annotate pixel-level labels.  
(4) **18** categories of labels, *e.g.*  face, sunglass, hat, scarf *etc*.  

[[homepage]](http://www.sysu-hcp.net/clothing-co-parsing-by-joint-image-segmentation-and-labeling/) [[pdf]](https://arxiv.org/pdf/1503.02391.pdf) 
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
**Fashion Icon 2015** 

(1) **Video dataset** and **Fashion Icon (FI) image dataset**.  
(2) Video dataset contains **1, 500** videos.  
(3) FI image dataset contains **1, 082** images, **18** categories.  

[[pdf]](https://liusi-group.com/pdf/Fashion%20Parsing%20with%20Video%20Context.pdf)
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
**Refined Fashionista 2017** :pig:  

(1) Reduces the number of clothing categories from **56** to **25** essential labels.  
(2) Manually annotated all the **685** images in the Fashionista dataset.  

[[homepage]](http://vision.is.tohoku.ac.jp/~kyamagu/research/clothing_parsing/) [[pdf]](https://arxiv.org/pdf/1703.01386.pdf) [[github]](https://github.com/pongsate1/fashion-parsing) 
```bib
@article{tangseng2017looking,
  title={Looking at outfit to parse clothing},
  author={Tangseng, Pongsate and Wu, Zhipeng and Yamaguchi, Kota},
  journal={arXiv preprint arXiv:1703.01386},
  year={2017}
}
```
**FASHION8 2018**   

(1) **9,339** fashion images from **8** continuous years are collected.  
(2) With human-annotated foreground masks.  

[[pdf]](https://arxiv.org/pdf/1803.03415.pdf)
```bib
@article{zhang2018fusing,
  title={Fusing Hierarchical Convolutional Features for Human Body Segmentation and Clothing Fashion Classification},
  author={Zhang, Zheng and Song, Chengfang and Zou, Qin},
  journal={arXiv preprint arXiv:1803.03415},
  year={2018}
}
```
- ModaNet 2018 [[homepage]](https://github.com/eBay/modanet) [[pdf]](https://arxiv.org/pdf/1807.01394.pdf) [[github]](https://github.com/hrsma2i/modanet) :pig:
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
- LandmarkDetection [[homepage]](http://mmlab.ie.cuhk.edu.hk/projects/DeepFashion/LandmarkDetection.html) [[pdf]](https://arxiv.org/pdf/1608.03049.pdf) [[github]](https://github.com/liuziwei7/fashion-landmarks) :pig:
```bib
@inproceedings{liu2016fashionlandmark,
 author = {Ziwei Liu, Sijie Yan, Ping Luo, Xiaogang Wang, and Xiaoou Tang},
 title = {Fashion Landmark Detection in the Wild},
 booktitle = {European Conference on Computer Vision (ECCV)},
 month = {October},
 year = {2016} 
}
```
- FASHIONAI Keypoint 2018 [[homepage]](https://tianchi.aliyun.com/competition/entrance/231648/introduction?lang=zh-cn) [[pdf]](http://openaccess.thecvf.com/content_CVPRW_2019/papers/FFSS-USAD/Zou_FashionAI_A_Hierarchical_Dataset_for_Fashion_Understanding_CVPRW_2019_paper.pdf) [[TIANCHI]]()
```bib
@inproceedings{zou2019fashionai,
  title={FashionAI: A Hierarchical Dataset for Fashion Understanding},
  author={Zou, Xingxing and Kong, Xiangheng and Wong, Waikeung and Wang, Congde and Liu, Yuguang and Cao, Yang},
  booktitle={Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition Workshops},
  pages={0--0},
  year={2019}
}
```
- DeepFashion2 2019 [[pdf]](https://arxiv.org/pdf/1901.07973.pdf) [[github]](https://github.com/switchablenorms/DeepFashion2) :pig:
```bib
@article{DeepFashion2,
  author = {Yuying Ge and Ruimao Zhang and Lingyun Wu and Xiaogang Wang and Xiaoou Tang and Ping Luo},
  title={A Versatile Benchmark for Detection, Pose Estimation, Segmentation and Re-Identification of Clothing Images},
  journal={CVPR},
  year={2019}
}
```

## 2. &nbsp;Attribute
For style analysis, attribute recognition, trend anaylsis, style anaylsis, multi-task learning, consumer-to-shop clothes retrieval, in-shop clothes retrieval and etc.
- Apparel Style 2012 [[homepage]](https://data.vision.ee.ethz.ch/cvl/lbossard/accv12/) [[pdf]](https://data.vision.ee.ethz.ch/cvl/lbossard/accv12/accv12_apparel-classification-with-style.pdf) :pig:
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
- WFC 2013 [[pdf]](https://www.cv-foundation.org/openaccess/content_cvpr_workshops_2013/W03/papers/Di_Style_Finder_Fine-Grained_2013_CVPR_paper.pdf)
```bib
@inproceedings{di2013style,
  title={Style finder: Fine-grained clothing style detection and retrieval},
  author={Di, Wei and Wah, Catherine and Bhardwaj, Anurag and Piramuthu, Robinson and Sundaresan, Neel},
  booktitle={Proceedings of the IEEE Conference on computer vision and pattern recognition workshops},
  pages={8--13},
  year={2013}
}
```
- ZOZOTOWN 2013 [[pdf]](https://www.researchgate.net/profile/Kiyoharu_Aizawa/publication/261438969_SNAPPER_Fashion_coordinate_image_retrieval_system/links/0f31753472d15b5839000000/SNAPPER-Fashion-coordinate-image-retrieval-system.pdf)
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
- Fashion136K 2013 [[pdf]](https://dl.acm.org/doi/pdf/10.1145/2623330.2623332)
```bib
@inproceedings{jagadeesh2014large,
  title={Large scale visual recommendations from street fashion images},
  author={Jagadeesh, Vignesh and Piramuthu, Robinson and Bhardwaj, Anurag and Di, Wei and Sundaresan, Neel},
  booktitle={Proceedings of the 20th ACM SIGKDD international conference on Knowledge discovery and data mining},
  pages={1925--1934},
  year={2014}
}
```
- UT-Zap50K 2014 [[homepage]](http://vision.cs.utexas.edu/projects/finegrained/utzap50k/) [[pdf]](http://aronyu.io/vision/papers/cvpr14/aron-cvpr14.pdf) :pig:
```bib
@InProceedings{finegrained,
  author = {A. Yu and K. Grauman},
  title = {Fine-Grained Visual Comparisons with Local Learning},
  booktitle = {Computer Vision and Pattern Recognition (CVPR)},
  month = {Jun},
  year = {2014}
}
```
- Fashion 10000 2014 [[homepage]](http://traces.cs.umass.edu/index.php/Mmsys/Mmsys) [[pdf]](https://dl.acm.org/doi/pdf/10.1145/2557642.2563675) :pig:
```bib
@inproceedings{loni2014fashion,
  title={Fashion 10000: an enriched social image dataset for fashion and clothing},
  author={Loni, Babak and Cheung, Lei Yen and Riegler, Michael and Bozzon, Alessandro and Gottlieb, Luke and Larson, Martha},
  booktitle={Proceedings of the 5th ACM Multimedia Systems Conference},
  pages={41--46},
  year={2014}
}
```
- Hipster Wars 2014 [[pdf]](https://projet.liris.cnrs.fr/imagine/pub/proceedings/ECCV-2014/papers/8689/86890472.pdf)
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
- Fashion144K 2015 [[homepage]](https://esslab.jp/~ess/en/data/fashion144k_stylenet/) [[pdf]](https://www.cs.toronto.edu/~urtasun/publications/simo_etal_cvpr15.pdf) :pig:
```bib
@InProceedings{SimoSerraCVPR2015,
  author    = {Edgar Simo-Serra and Sanja Fidler and Francesc Moreno-Noguer and Raquel Urtasun},
  title     = {{Neuroaesthetics in Fashion: Modeling the Perception of Fashionability}},
  booktitle = "Proceedings of the Conference on Computer Vision and Pattern Recognition (CVPR)",
  year      = 2015,
}
```
- WITB 2015 [[homepage]](http://www.tamaraberg.com/street2shop/) [[pdf]](http://www.tamaraberg.com/papers/street2shop.pdf) :pig:
```bib
@inproceedings{hadi2015buy,
  title={Where to buy it: Matching street clothing photos in online shops},
  author={Hadi Kiapour, M and Han, Xufeng and Lazebnik, Svetlana and Berg, Alexander C and Berg, Tamara L},
  booktitle={Proceedings of the IEEE international conference on computer vision},
  pages={3343--3351},
  year={2015}
}
```
- DARN 2015 [[pdf]](https://www.cv-foundation.org/openaccess/content_iccv_2015/papers/Huang_Cross-Domain_Image_Retrieval_ICCV_2015_paper.pdf)
```bib
@inproceedings{huang2015cross,
  title={Cross-domain image retrieval with a dual attribute-aware ranking network},
  author={Huang, Junshi and Feris, Rogerio S and Chen, Qiang and Yan, Shuicheng},
  booktitle={Proceedings of the IEEE international conference on computer vision},
  pages={1062--1070},
  year={2015}
}
```
- Clothing1M 2015 [[pdf]](https://www.ee.cuhk.edu.hk/~xgwang/papers/xiaoXYHWcvpr15.pdf) [[github]](https://github.com/Cysu/noisy_label) :pig:
```bib
@inproceedings{xiao2015learning,
  title={Learning from Massive Noisy Labeled Data for Image Classification},
  author={Xiao, Tong and Xia, Tian and Yang, Yi and Huang, Chang and Wang, Xiaogang},
  booktitle={CVPR},
  year={2015}
}
```
- YahooClothing 2015 [[pdf]](https://dl.acm.org/doi/pdf/10.1145/2671188.2749318)
```bib
@inproceedings{lin2015rapid,
  title={Rapid clothing retrieval via deep learning of binary codes and hierarchical search},
  author={Lin, Kevin and Yang, Huei-Fang and Liu, Kuan-Hsien and Hsiao, Jen-Hao and Chen, Chu-Song},
  booktitle={Proceedings of the 5th ACM on International Conference on Multimedia Retrieval},
  pages={499--502},
  year={2015}
}
```
- Chitopia 2015 [[pdf]](http://www.bmva.org/bmvc/2015/papers/paper051/paper051.pdf)
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
- Etsy | Wear 2016 [[homepage]](http://vision.is.tohoku.ac.jp/~kyamagu/research/etsy-dataset/) [[pdf]](https://arxiv.org/pdf/1607.07262.pdf) :pig:
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
- DeepFashion 2016 [[homepage]](http://mmlab.ie.cuhk.edu.hk/projects/DeepFashion.html) [[pdf]](https://www.ee.cuhk.edu.hk/~xgwang/papers/liuLQWTcvpr16.pdf) :pig:
```bib
@inproceedings{liuLQWTcvpr16DeepFashion,
 author = {Liu, Ziwei and Luo, Ping and Qiu, Shi and Wang, Xiaogang and Tang, Xiaoou},
 title = {DeepFashion: Powering Robust Clothes Recognition and Retrieval with Rich Annotations},
 booktitle = {Proceedings of IEEE Conference on Computer Vision and Pattern Recognition (CVPR)},
 month = {June},
 year = {2016} 
 }
 ```
- MVC 2016 [[homepage]](http://mvc-datasets.github.io/MVC/) [[pdf]](https://www.iis.sinica.edu.tw/papers/song/19692-F.pdf) [[github]](https://github.com/MVC-Datasets/MVC) :pig:
```bib
@inproceedings{liu2016mvc,
  title={Mvc: A dataset for view-invariant clothing retrieval and attribute prediction},
  author={Liu, Kuan-Hsien and Chen, Ting-Yen and Chen, Chu-Song},
  booktitle={Proceedings of the 2016 ACM on International Conference on Multimedia Retrieval},
  pages={313--316},
  year={2016}
}
```
- StreetStyle27K 2017 [[homepage]](http://streetstyle.cs.cornell.edu/#dataset) [[pdf]](https://arxiv.org/pdf/1706.01869.pdf) :pig:
```bib
@article{StreetStyle2017,
  title={{StreetStyle}: {E}xploring world-wide clothing styles from millions of photos},
  author={Kevin Matzen and Kavita Bala and Noah Snavely},
  journal={arXiv preprint arXiv:1706.01869},
  year={2017}
}
```
- Fashionstyle14 2017 [[homepage]](https://esslab.jp/~ess/en/data/fashionstyle14/) [[pdf]](http://openaccess.thecvf.com/content_ICCV_2017_workshops/papers/w32/Takagi_What_Makes_a_ICCV_2017_paper.pdf) :pig:
```bib
@inproceedings{takagi2017makes,
  title={What makes a style: Experimental analysis of fashion prediction},
  author={Takagi, Moeko and Simo-Serra, Edgar and Iizuka, Satoshi and Ishikawa, Hiroshi},
  booktitle={Proceedings of the IEEE International Conference on Computer Vision Workshops},
  pages={2247--2253},
  year={2017}
}
```
- Fashion200K 2017 [[pdf]](http://openaccess.thecvf.com/content_ICCV_2017/papers/Han_Automatic_Spatially-Aware_Fashion_ICCV_2017_paper.pdf) [[github]](https://github.com/xthan/fashion-200k/) :pig:
```bib
@inproceedings{han2017automatic,
  title = {Automatic Spatially-aware Fashion Concept Discovery},
  author = {Han, Xintong and Wu, Zuxuan and Huang, Phoenix X. and Zhang, Xiao and Zhu, Menglong and Li, Yuan and Zhao, Yang  and Davis, Larry S.},
  booktitle = {ICCV},
  year  = {2017},
}
```
- Fashion550K 2017 [[homepage]](https://esslab.jp/~ess/en/data/fashion550k/) [[pdf]](http://openaccess.thecvf.com/content_ICCV_2017_workshops/papers/w32/Inoue_Multi-Label_Fashion_Image_ICCV_2017_paper.pdf) :pig:
```bib
@InProceedings{InoueICCVW2017,
   author    = {Naoto Inoue and Edgar Simo-Serra and Toshihiko Yamasaki and Hiroshi Ishikawa},
   title     = {{Multi-Label Fashion Image Classification with Minimal Human Supervision}},
   booktitle = "Proceedings of the International Conference on Computer Vision Workshops (ICCVW)",
   year      = 2017,
}
```
- Amazon Dress [[pdf]](https://kddfashion2017.mybluemix.net/final_submissions/ML4Fashion_paper_7.pdf)
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
- SFS 2017 [[homepage]](https://zenodo.org/record/833051#.XqfGivmWa70) [[pdf]](http://doi.org/10.1145/3123266.3123441) :pig:
```bib
@inproceedings{gu2017understanding,
  title={Understanding fashion trends from street photos via neighbor-constrained embedding learning},
  author={Gu, Xiaoling and Wong, Yongkang and Peng, Pai and Shou, Lidan and Chen, Gang and Kankanhalli, Mohan S},
  booktitle={Proceedings of the 25th ACM international conference on Multimedia},
  pages={190--198},
  year={2017}
}
```
- Video2Shop 2017 [[pdf]](http://openaccess.thecvf.com/content_cvpr_2017/papers/Cheng_Video2Shop_Exact_Matching_CVPR_2017_paper.pdf)
```bib
@inproceedings{cheng2017video2shop,
  title={Video2shop: Exact matching clothes in videos to online shopping images},
  author={Cheng, Zhi-Qi and Wu, Xiao and Liu, Yang and Hua, Xian-Sheng},
  booktitle={Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition},
  pages={4048--4056},
  year={2017}
}
```
- RFS | PFS 2018 
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
- BrandFashion 2018 [[pdf]](http://openaccess.thecvf.com/content_ECCVW_2018/papers/11131/Manandhar_Tiered_Deep_Similarity_Search_for_Fashion_ECCVW_2018_paper.pdf)
```bib
@inproceedings{manandhar2018tiered,
  title={Tiered Deep Similarity Search for Fashion},
  author={Manandhar, Dipu and Bastan, Muhammet and Yap, Kim-Hui},
  booktitle={Proceedings of the European Conference on Computer Vision (ECCV)},
  pages={0--0},
  year={2018}
}
```
- FashionBrand 2018 [[pdf]](https://arxiv.org/pdf/1810.09941v1.pdf)
```bib
@inproceedings{hadi2018brand,
  title={Brand> Logo: Visual Analysis of Fashion Brands},
  author={Hadi Kiapour, M and Piramuthu, Robinson},
  booktitle={Proceedings of the European Conference on Computer Vision (ECCV)},
  pages={0--0},
  year={2018}
}
```
- Fashion60 2018 [[link]](https://ieeexplore.ieee.org/document/8396968)
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
- X-domain 2018 [[pdf]](https://arxiv.org/pdf/1804.10851.pdf)
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
- Women | Men Video 2018 [[pdf]](https://www.researchgate.net/profile/Sanyi_Zhang/publication/321785076_Watch_Fashion_Shows_to_Tell_Clothing_Attributes/links/5cdf0e3c92851c4eabaa3e07/Watch-Fashion-Shows-to-Tell-Clothing-Attributes.pdf)
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
- FASHIONAI Attributes 2018 [[homepage]](https://tianchi.aliyun.com/competition/entrance/231649/information) [[pdf]](http://openaccess.thecvf.com/content_CVPRW_2019/papers/FFSS-USAD/Zou_FashionAI_A_Hierarchical_Dataset_for_Fashion_Understanding_CVPRW_2019_paper.pdf) [[TIANCHI]]()
```bib
@inproceedings{zou2019fashionai,
  title={FashionAI: A Hierarchical Dataset for Fashion Understanding},
  author={Zou, Xingxing and Kong, Xiangheng and Wong, Waikeung and Wang, Congde and Liu, Yuguang and Cao, Yang},
  booktitle={Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition Workshops},
  pages={0--0},
  year={2019}
}
```
- Feidegger 2018 [[homepage]](https://research.zalando.com/welcome/mission/research-projects/feidegger-dataset/) [[pdf]](http://www.lrec-conf.org/proceedings/lrec2018/pdf/319.pdf)
```bib
@inproceedings{lefakis2018feidegger,
  title={FEIDEGGER: A Multi-modal Corpus of Fashion Images and Descriptions in German},
  author={Lefakis, Leonidas and Akbik, Alan and Vollgraf, Roland},
  booktitle={Proceedings of the Eleventh International Conference on Language Resources and Evaluation (LREC 2018)},
  year={2018}
}
```
- Studio2Shop 2018 [[pdf]](https://www.scitepress.org/Papers/2018/65445/65445.pdf)
```bib
@article{lasserre2018studio2shop,
  title={Studio2shop: from studio photo shoots to fashion articles},
  author={Lasserre, Julia and Rasch, Katharina and Vollgraf, Roland},
  journal={arXiv preprint arXiv:1807.00556},
  year={2018}
}
```
- Shopping 100k 2018 [[pdf]](https://www.researchgate.net/profile/Kenan_Ak/publication/324728522_Efficient_Multi-Attribute_Similarity_Learning_Towards_Attribute-based_Fashion_Search/links/5adf5078aca272fdaf89c65a/Efficient-Multi-Attribute-Similarity-Learning-Towards-Attribute-based-Fashion-Search.pdf)
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
- Footwear 2018 [[homepage]](https://www.cse.iitd.ac.in/~chetan/projects.html) [[pdf]](https://www.cse.iitd.ac.in/~chetan/papers/icip18-fgvc.pdf)
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
- iMaterialist 2019 [[homepage]](https://www.kaggle.com/c/imaterialist-fashion-2019-FGVC6) [[pdf]](http://openaccess.thecvf.com/content_ICCVW_2019/papers/CVFAD/Guo_The_iMaterialist_Fashion_Attribute_Dataset_ICCVW_2019_paper.pdf) [[github]](https://github.com/visipedia/imat_fashion_comp) :pig:
```bib
@inproceedings{guo2019imaterialist,
  title={The imaterialist fashion attribute dataset},
  author={Guo, Sheng and Huang, Weilin and Zhang, Xiao and Srikhanta, Prasanna and Cui, Yin and Li, Yuan and Adam, Hartwig and Scott, Matthew R and Belongie, Serge},
  booktitle={Proceedings of the IEEE International Conference on Computer Vision Workshops},
  pages={0--0},
  year={2019}
}
```
- Atlas 2019 [[homepage]](https://github.com/vumaasha/atlas) [[pdf]](https://arxiv.org/pdf/1908.08984.pdf) :pig:
```bib
@article{umaashankar2019atlas,
  title={Atlas: A Dataset and Benchmark for E-commerce Clothing Product Categorization},
  author={Umaashankar, Venkatesh and Prakash, Aditi and others},
  journal={arXiv preprint arXiv:1908.08984},
  year={2019}
}
```
- DeepShoe 2019 [[pdf]](http://alumni.media.mit.edu/~shiboxin/files/Zhan_CVIU19.pdf)
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
- FindFashion 2019 combine DeepFashion & Street2Shop [[pdf]](http://openaccess.thecvf.com/content_ICCV_2019/papers/Kuang_Fashion_Retrieval_via_Graph_Reasoning_Networks_on_a_Similarity_Pyramid_ICCV_2019_paper.pdf) 
```bib
@inproceedings{kuang2019fashion,
  title={Fashion Retrieval via Graph Reasoning Networks on a Similarity Pyramid},
  author={Kuang, Zhanghui and Gao, Yiming and Li, Guanbin and Luo, Ping and Chen, Yimin and Lin, Liang and Zhang, Wayne},
  booktitle={Proceedings of the IEEE International Conference on Computer Vision},
  pages={3066--3075},
  year={2019}
}
```
- GarmentSet 2020 [[pdf]](https://arxiv.org/pdf/2001.06427.pdf)
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
- WoW 2012 [[pdf]](https://dl.acm.org/doi/pdf/10.1145/2393347.2393433)
```bib
@inproceedings{liu2012hi,
  title={Hi, magic closet, tell me what to wear!},
  author={Liu, Si and Feng, Jiashi and Song, Zheng and Zhang, Tianzhu and Lu, Hanqing and Xu, Changsheng and Yan, Shuicheng},
  booktitle={Proceedings of the 20th ACM international conference on Multimedia},
  pages={619--628},
  year={2012}
}
```
- Stylatrix
```bib
@article{sunstylatrix,
  title={Stylatrix: an interactive model-based system for fashion exploration and outfit discovery},
  author={Sun, Will J and Gajos, Krzysztof Z}
}
```
- Edge2Garment 2016 [[homepage]](https://phillipi.github.io/pix2pix/) [[pdf]](https://arxiv.org/pdf/1810.09941v1.pdf) [[github]](https://github.com/phillipi/pix2pix) [[datalink]](https://people.eecs.berkeley.edu/~tinghuiz/projects/pix2pix/datasets/) :pig:
```bib
@article{pix2pix2016,
  title={Image-to-Image Translation with Conditional Adversarial Networks},
  author={Isola, Phillip and Zhu, Jun-Yan and Zhou, Tinghui and Efros, Alexei A},
  journal={arxiv},
  year={2016}
}
```
- FashionVC 2017 [[pdf]](https://dl.acm.org/doi/pdf/10.1145/3123266.3123314)
```bib
@inproceedings{song2017neurostylist,
  title={Neurostylist: Neural compatibility modeling for clothing matching},
  author={Song, Xuemeng and Feng, Fuli and Liu, Jinhuan and Li, Zekun and Nie, Liqiang and Ma, Jun},
  booktitle={Proceedings of the 25th ACM international conference on Multimedia},
  pages={753--761},
  year={2017}
}
```
- Fashion409K 2017 [[homepage]](http://vision.is.tohoku.ac.jp/~tangseng/smart_closet_project.html) [[pdf]](http://openaccess.thecvf.com/content_ICCV_2017_workshops/papers/w32/Tangseng_Recommending_Outfits_From_ICCV_2017_paper.pdf) :pig:
```bib
@InProceedings{Tangseng_2017_ICCV,
author = {Tangseng, Pongsate and Yamaguchi, Kota and Okatani, Takayuki},
title = {Recommending Outfits From Personal Closet},
booktitle = {The IEEE International Conference on Computer Vision (ICCV) Workshops},
month = {Oct},
year = {2017}
}
```
- Polyvore 2017 [[pdf]](https://arxiv.org/pdf/1707.05691.pdf) [[github]](https://github.com/xthan/polyvore) :pig:
```bib
@inproceedings{han2017learning,
  author = {Han, Xintong and Wu, Zuxuan and Jiang, Yu-Gang and Davis, Larry S},
  title = {Learning Fashion Compatibility with Bidirectional LSTMs},
  booktitle = {ACM Multimedia},
  year  = {2017},
}
```
- AVA 2017 [[homepage]](http://personal.ie.cuhk.edu.hk/~dy015/ImageAesthetics/Image_Aesthetic_Assessment.html) [[pdf]](https://arxiv.org/pdf/1610.00838.pdf) :pig:
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
- UIUC 2018 [[pdf]](http://openaccess.thecvf.com/content_ECCV_2018/papers/Mariya_Vasileva_Learning_Type-Aware_Embeddings_ECCV_2018_paper.pdf) [[github]](https://github.com/mvasil/fashion-compatibility) 
```bib
@inproceedings{VasilevaECCV18FasionCompatibility,
Author = {Mariya I. Vasileva and Bryan A. Plummer and Krishna Dusad and Shreya Rajpal and Ranjitha Kumar and David Forsyth},
Title = {Learning Type-Aware Embeddings for Fashion Compatibility},
booktitle = {ECCV},
Year = {2018}
}
```
- IQON 2018 [[pdf]](https://arxiv.org/pdf/1807.03133.pdf) [[github]](https://github.com/Cherrybruin/iqon-dataset)
```bib
@article{nakamura2018outfit,
  title={Outfit generation and style extraction via bidirectional lstm and autoencoder},
  author={Nakamura, Takuma and Goto, Ryosuke},
  journal={arXiv preprint arXiv:1807.03133},
  year={2018}
}
```
- Style4BodyShape 2018 [[pdf]](https://dl.acm.org/doi/pdf/10.1145/3240508.3240546)
```bib
@inproceedings{hidayati2018dress,
  title={What dress fits me best? fashion recommendation on the clothing style for personal body shape},
  author={Hidayati, Shintami Chusnul and Hsu, Cheng-Chun and Chang, Yu-Ting and Hua, Kai-Lung and Fu, Jianlong and Cheng, Wen-Huang},
  booktitle={Proceedings of the 26th ACM international conference on Multimedia},
  pages={438--446},
  year={2018}
}
```
- Lookastic 2019 [[pdf]](http://staff.ustc.edu.cn/~hexn/papers/sigir19-fashion.pdf)
```bib
@inproceedings{yang2019interpretable,
  title={Interpretable Fashion Matching with Rich Attributes},
  author={Yang, Xun and He, Xiangnan and Wang, Xiang and Ma, Yunshan and Feng, Fuli and Wang, Meng and Chua, Tat-Seng},
  booktitle={Proceedings of the 42nd International ACM SIGIR Conference on Research and Development in Information Retrieval},
  pages={775--784},
  year={2019}
}
```
- POG 2019 [[pdf]](https://arxiv.org/pdf/1905.01866.pdf) [[github]](https://github.com/wenyuer/POG) :pig:
```bib
@inproceedings{chen2019pog,
  title={POG: Personalized Outfit Generation for Fashion Recommendation at Alibaba iFashion},
  author={Chen, Wen and Huang, Pipei and Xu, Jiaming and Guo, Xin and Guo, Cheng and Sun, Fei and Li, Chao and Pfadler, Andreas and Zhao, Huan and Zhao, Binqiang},
  booktitle={Proceedings of the 25th ACM SIGKDD International Conference on Knowledge Discovery \& Data Mining},
  pages={2662--2670},
  year={2019}
}
```
- Shop the Look 2019 [[pdf]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Kang_Complete_the_Look_Scene-Based_Complementary_Product_Recommendation_CVPR_2019_paper.pdf)[[github]](https://github.com/kang205/STL-Dataset) 
```bib
@inproceedings{kang2019complete,
  title={Complete the Look: Scene-based Complementary Product Recommendation},
  author={Kang, Wang-Cheng and Kim, Eric and Leskovec, Jure and Rosenberg, Charles and McAuley, Julian},
  booktitle={Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition},
  pages={10532--10541},
  year={2019}
}
```
- ExpFashion 2019 [[pdf]](https://xuemengsong.github.io/Neuro_2019.pdf)
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
- ASOS outfits 2019 [[pdf]](https://arxiv.org/pdf/1904.00741.pdf)
```bib
@article{bettaney2019fashion,
  title={Fashion Outfit Generation for E-commerce},
  author={Bettaney, Elaine M and Hardwick, Stephen R and Zisimopoulos, Odysseas and Chamberlain, Benjamin Paul},
  journal={arXiv preprint arXiv:1904.00741},
  year={2019}
}
```
- Chuanda 2020 [[pdf]](https://arxiv.org/pdf/2004.06229.pdf)
```bib
@article{liu2020imitation,
  title={Imitation Learning for Fashion Style Based on Hierarchical Multimodal Representation},
  author={Liu, Shizhu and Yang, Shanglin and Zhou, Hui},
  journal={arXiv preprint arXiv:2004.06229},
  year={2020}
}
```

## 4. &nbsp;Generation
- MPI Dynamic FAUST | BUFF 2017 [[homepage]](http://buff.is.tue.mpg.de/) [[pdf]](http://openaccess.thecvf.com/content_cvpr_2017/papers/Bogo_Dynamic_FAUST_Registering_CVPR_2017_paper.pdf) :pig:
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
- FashionGAN 2017 [[pdf]](http://openaccess.thecvf.com/content_ICCV_2017/papers/Zhu_Be_Your_Own_ICCV_2017_paper.pdf) [[github]](https://github.com/zhusz/ICCV17-fashionGAN) :pig:
```bib
@inproceedings{zhu2017be,
  title={Be Your Own Prada: Fashion Synthesis with Structural Coherence},
  author={Zhu, Shizhan and Fidler, Sanja and Urtasun, Raquel and Lin, Dahua and Chen, Change Loy},
  booktitle={Proceedings of the IEEE Conference on International Conference on Computer Vision},
  year={2017}
}
```
- BeautyGAN 2018 [[homepage]](http://liusi-group.com/projects/BeautyGAN) [[pdf]](https://dl.acm.org/doi/pdf/10.1145/3240508.3240618) :pig:
```bib
@inproceedings{li2018beautygan,
  title={Beautygan: Instance-level facial makeup transfer with deep generative adversarial network},
  author={Li, Tingting and Qian, Ruihe and Dong, Chao and Liu, Si and Yan, Qiong and Zhu, Wenwu and Lin, Liang},
  booktitle={Proceedings of the 26th ACM international conference on Multimedia},
  pages={645--653},
  year={2018}
}
```
- VTON 2018 [[pdf]](http://openaccess.thecvf.com/content_cvpr_2018/papers/Han_VITON_An_Image-Based_CVPR_2018_paper.pdf) [[github]](https://github.com/xthan/VITON) 
```bib
@inproceedings{han2017viton,
  title = {VITON: An Image-based Virtual Try-on Network},
  author = {Han, Xintong and Wu, Zuxuan and Wu, Zhe and Yu, Ruichi and Davis, Larry S},
  booktitle = {CVPR},
  year  = {2018},
}
```
- DeepWear 2018 [[pdf]](https://digitalnature.slis.tsukuba.ac.jp/wp-content/uploads/2018/03/deepwear.pdf)
```bib
@inproceedings{kato2018deepwear,
  title={DeepWear: a Case Study of Collaborative Design between Human and Artificial Intelligence},
  author={Kato, Natsumi and Osone, Hiroyuki and Sato, Daitetsu and Muramatsu, Naoya and Ochiai, Yoichi},
  booktitle={Proceedings of the Twelfth International Conference on Tangible, Embedded, and Embodied Interaction},
  pages={529--536},
  year={2018}
}
```
- FashionGEN 2018 [[homepage]](https://fashion-gen.com/) [[pdf]](https://arxiv.org/pdf/1806.08317.pdf)
```bib
@article{rostamzadeh2018fashion,
  title={Fashion-gen: The generative fashion dataset and challenge},
  author={Rostamzadeh, Negar and Hosseini, Seyedarian and Boquet, Thomas and Stokowiec, Wojciech and Zhang, Ying and Jauvin, Christian and Pal, Chris},
  journal={arXiv preprint arXiv:1806.08317},
  year={2018}
}
```
- ZalandoGAN 2018 [[homepage]](https://research.zalando.com/welcome/mission/research-projects/generative-fashion-design/) [[pdf]](https://arxiv.org/pdf/1806.07819.pdf) [[github]](https://github.com/zalandoresearch/disentangling_conditional_gans)
```bib
@article{yildirim2018disentangling,
  title={Disentangling multiple conditional inputs in gans},
  author={Yildirim, G{\"o}khan and Seward, Calvin and Bergmann, Urs},
  journal={arXiv preprint arXiv:1806.07819},
  year={2018}
}
```
- RTW 2018 [[pdf]](http://openaccess.thecvf.com/content_ECCVW_2018/papers/11131/Sbai_DesIGN_Design_Inspiration_from_Generative_Networks_ECCVW_2018_paper.pdf)
```bib
@inproceedings{sbai2018design,
  title={Design: Design inspiration from generative networks},
  author={Sbai, Othman and Elhoseiny, Mohamed and Bordes, Antoine and LeCun, Yann and Couprie, Camille},
  booktitle={Proceedings of the European Conference on Computer Vision (ECCV)},
  pages={0--0},
  year={2018}
}
```
- SMPL 2018 [[homepage]](https://www.epfl.ch/labs/cvlab/research/garment-simulation/garnet/) [[pdf]](http://openaccess.thecvf.com/content_ICCV_2019/papers/Gundogdu_GarNet_A_Two-Stream_Network_for_Fast_and_Accurate_3D_Cloth_ICCV_2019_paper.pdf) 
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
- Fashion Takes 2019 [[pdf]](https://virtualhumans.mpi-inf.mpg.de/papers/sattar2019WACV/sattar2019WACV.pdf)
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
- StyleGAN 2019 [[pdf]](http://openaccess.thecvf.com/content_ICCVW_2019/papers/CVFAD/Yildirim_Generating_High-Resolution_Fashion_Model_Images_Wearing_Custom_Outfits_ICCVW_2019_paper.pdf)
```bib
@inproceedings{yildirim2019generating,
  title={Generating High-Resolution Fashion Model Images Wearing Custom Outfits},
  author={Yildirim, Gokhan and Jetchev, Nikolay and Vollgraf, Roland and Bergmann, Urs},
  booktitle={Proceedings of the IEEE International Conference on Computer Vision Workshops},
  pages={0--0},
  year={2019}
}
```
- Deep Fashion3D 2020 [[pdf]](https://arxiv.org/pdf/2003.12753.pdf)
```bib
@article{zhu2020deep,
  title={Deep Fashion3D: A Dataset and Benchmark for 3D Garment Reconstruction from Single Images},
  author={Zhu, Heming and Cao, Yu and Jin, Hang and Chen, Weikai and Du, Dong and Wang, Zhangye and Cui, Shuguang and Han, Xiaoguang},
  journal={arXiv preprint arXiv:2003.12753},
  year={2020}
}
```

## 5. &nbsp;Others
- Amazon Reviews 2015 [[homepage]](https://nijianmo.github.io/amazon/index.html) [[pdf]](https://dl.acm.org/doi/pdf/10.1145/2766462.2767755)
```bib
@inproceedings{mcauley2015image,
  title={Image-based recommendations on styles and substitutes},
  author={McAuley, Julian and Targett, Christopher and Shi, Qinfeng and Van Den Hengel, Anton},
  booktitle={Proceedings of the 38th International ACM SIGIR Conference on Research and Development in Information Retrieval},
  pages={43--52},
  year={2015}
}
```
- Tradesy 2016 [[homepage]](http://jmcauley.ucsd.edu/data/tradesy/) [[pdf]](http://cseweb.ucsd.edu/~jmcauley/pdfs/aaai16.pdf) :pig:
```bib
@inproceedings{he2016vbpr,
  title={VBPR: visual bayesian personalized ranking from implicit feedback},
  author={He, Ruining and McAuley, Julian},
  booktitle={Thirtieth AAAI Conference on Artificial Intelligence},
  year={2016}
}
```
- Fashion-MNIST 2017 [[homepage]](https://research.zalando.com/welcome/mission/research-projects/fashion-mnist/) [[pdf]](https://arxiv.org/pdf/1708.07747.pdf) [[github]](https://github.com/zalandoresearch/fashion-mnist) :pig:
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
- Shoe 2018 [[pdf]](http://papers.nips.cc/paper/7348-dialog-based-interactive-image-retrieval.pdf)
```bib
@inproceedings{guo2018dialog,
  title={Dialog-based interactive image retrieval},
  author={Guo, Xiaoxiao and Wu, Hui and Cheng, Yu and Rennie, Steven and Tesauro, Gerald and Feris, Rogerio},
  booktitle={Advances in Neural Information Processing Systems},
  pages={678--688},
  year={2018}
}
```
- Flickr30k 2018 [[pdf]](https://dl.acm.org/doi/pdf/10.1145/3184558.3186354)
```bib
@inproceedings{lin2018netizen,
  title={Netizen-style commenting on fashion photos: dataset and diversity measures},
  author={Lin, Wen Hua and Chen, Kuan-Ting and Chiang, Hung Yueh and Hsu, Winston},
  booktitle={Companion Proceedings of the The Web Conference 2018},
  pages={395--402},
  year={2018}
}
```
- FCDB 2019 [[homepage]](http://hirokatsukataoka.net/) [[pdf]](http://openaccess.thecvf.com/content_CVPRW_2019/papers/FFSS-USAD/Kataoka_Ten-Million-Order_Human_Database_for_World-Wide_Fashion_Culture_Analysis_CVPRW_2019_paper.pdf) [[github]](https://github.com/cvpaperchallenge/FashionCultureDataBase_DLoader) :pig:
```bib
@InProceedings{Kataoka_2019_CVPR_Workshops,
author = {Kataoka, Hirokatsu and Satoh, Yutaka and Abe, Kaori and Minoguchi, Munetaka and Nakamura, Akio},
title = {Ten-Million-Order Human Database for World-Wide Fashion Culture Analysis},
booktitle = {The IEEE Conference on Computer Vision and Pattern Recognition (CVPR) Workshops},
month = {June},
year = {2019}
}
```
- Fashion IQ 2019 [[pdf]](https://arxiv.org/pdf/1905.12794.pdf) [[github]](https://github.com/XiaoxiaoGuo/fashion-iq) [[github]](https://github.com/XiaoxiaoGuo/fashion-iq) :pig:
```bib
@article{guo2019fashion,
  title={The Fashion IQ Dataset: Retrieving Images by Combining Side Information and Relative Natural Language Feedback},
  author={Guo, Xiaoxiao and Wu, Hui and Gao, Yupeng and Rennie, Steven and Feris, Rogerio},
  journal={arXiv preprint arXiv:1905.12794},
  year={2019}
}
```
- TFCD 2019 [[pdf]](https://arxiv.org/ftp/arxiv/papers/1907/1907.00400.pdf)
```bib
@article{bigon2019prediction,
  title={Prediction is very hard, especially about conversion. Predicting user purchases from clickstream data in fashion e-commerce},
  author={Bigon, Luca and Cassani, Giovanni and Greco, Ciro and Lacasa, Lucas and Pavoni, Mattia and Polonioli, Andrea and Tagliabue, Jacopo},
  journal={arXiv preprint arXiv:1907.00400},
  year={2019}
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
Here I would like to thank Miss Boey Pang, Miss Selene Lee, for their hard work on collecting datasource information.
