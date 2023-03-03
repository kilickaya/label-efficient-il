# Towards Label-Efficient Incremental Learning: A Survey

[Paper](https://arxiv.org/pdf/2302.00353.pdf) | [Slides](https://kilickaya.github.io/resume/survey.pdf)

Please cite the following bib entry in case you use it:
```
@article{kilickaya2023towards,
    author = {Kilickaya, Mert and Van der Weijer, Joost and Asano, Yuki},
    title = {Towards Label-Efficient Incremental Learning: A Survey},
    journal = {arXiv preprint arXiv:2302.00353},
    year = {2023}
}
```

You have a cool paper you think we should consider? Please open an [issue](https://github.com/kilickaya/label-efficient-il/issues/new/choose) or send me an [e-mail](kilickayamert@gmail.com).   

**Abstract**: The current dominant paradigm when building a
machine learning model is to iterate over a dataset
over and over until convergence. Such an approach is non-incremental, as it assumes access
to all images of all categories at once. However,
for many applications, non-incremental learning
is unrealistic. To that end, researchers study incremental learning, where a learner is required to
adapt to an incoming stream of data with a varying distribution while preventing forgetting of past
knowledge. Significant progress has been made,
however, the vast majority of works focus on the
fully supervised setting, making these algorithms
label-hungry thus limiting their real-life deployment. To that end, in this paper, we make the
first attempt to survey recently growing interest
in label-efficient incremental learning. We identify three subdivisions, namely semi-, few-shotand self-supervised learning to reduce labeling efforts. Finally, we identify novel directions that
can further enhance label-efficiency and improve
incremental learning scalability

## Flowchart
![summary](https://user-images.githubusercontent.com/8891413/222820805-4597104c-2e1d-4d0d-b818-b8187d6ce94c.PNG)
Here, we compare three different paradigms for label-efficient incremental learning. 

## Summary

![summary2](https://user-images.githubusercontent.com/8891413/222820855-7590786c-87d8-4854-8e59-2969802e46d1.PNG)

Here, we summarize main settings studied for label-efficient incremental learning. 

## Semi-Supervision for Incremental Learning

| Algorithm | Setting | Year | Code | 
| -------- | -------- | -------- | -------- |
| [CNLL](https://dl.acm.org/doi/10.1145/3094243.3094247)      | Within | 2017 | - |
| [DistillMatch](https://arxiv.org/abs/2101.09536) | Within | 2021 | [Code](https://github.com/GT-RIPL/DistillMatch-SSCL) |
| [ORDisCo](https://arxiv.org/abs/2101.00407) | Within | 2021 | - |
| [MetaCon](https://arxiv.org/abs/2110.01856) | Within | 2021 | - | 
| [PGL](https://arxiv.org/abs/2201.09196) | Within | 2022 | [Code](https://github.com/luoyan407/grad_prediction) |
| [NNCSL](https://arxiv.org/pdf/2212.05102.pdf) | Within | 2022 | [Code](https://github.com/kangzhiq/NNCSL)
| [DMC](https://arxiv.org/abs/1903.07864) | Auxiliary | 2020 | - |
| [CIL-QUD](https://arxiv.org/abs/2206.07842) | Auxiliary | 2022 | [Code](https://github.com/VITA-Group/CIL-QUD) | 
| [CoTTA](https://arxiv.org/abs/2203.13591) | Test | 2022 | [Code](https://github.com/qinenergy/cotta) | 
| [NOTE](https://arxiv.org/abs/2208.05117) | Test  | 2022 | [Code](https://github.com/TaesikGong/NOTE) | 



## Few-shot-Supervision for Incremental Learning

| Algorithm | Setting | Year | Code | 
| -------- | -------- | -------- | -------- |
| [TOPIC](https://openaccess.thecvf.com/content_CVPR_2020/papers/Tao_Few-Shot_Class-Incremental_Learning_CVPR_2020_paper.pdf) | Graph | 2020  | - | 
| [CEC](https://openaccess.thecvf.com/content/CVPR2021/papers/Zhang_Few-Shot_Incremental_Learning_With_Continually_Evolved_Classifiers_CVPR_2021_paper.pdf) | Graph | 2021 | - | 
| [IDL-VQ](https://openreview.net/forum?id=3SV-ZePhnZM) | Clustering | 2020 | - | 
| [SA-KD](https://arxiv.org/abs/2103.04059) | Clustering | 2021 | - | 
| [Sub-Reg](https://openreview.net/forum?id=boJy41J-tnQ) | Clustering | 2020 | [Code](https://github.com/feyzaakyurek/subspace-reg) | 
| [FACT](https://arxiv.org/abs/2203.06953) | Clustering | 2022 | [Code](https://github.com/zhoudw-zdw/CVPR22-Fact) | 
| [NCollapse](https://arxiv.org/pdf/2302.03004.pdf) | Clustering | 2023 | [Code](https://github.com/NeuralCollapseApplications/FSCIL)
| [FSLL](https://arxiv.org/pdf/2103.00991.pdf) | Architectural | 2021 | - | 
| [C-FSCIL](https://arxiv.org/abs/2203.16588) | Architectural | 2022 | [Code](https://github.com/IBM/constrained-FSCIL) | 


## Self-Supervision for Incremental Learning

| Algorithm | Setting | Year | Code | 
| -------- | -------- | -------- | -------- |
| [SSL-OCL](https://arxiv.org/pdf/2103.14010.pdf) | Pre-training | 2021 | - | 
| [PASS](https://openaccess.thecvf.com/content/CVPR2021/papers/Zhu_Prototype_Augmentation_and_Self-Supervision_for_Incremental_Learning_CVPR_2021_paper.pdf) | Auxiliary-training | 2021 | - | 
| [Buffer-SSL](https://arxiv.org/abs/2203.12710) | Main-training | 2022 | - | 
| [LUMP](https://openreview.net/forum?id=9Hrka5PA7LW) | Main-training | 2022 | [Code](https://github.com/divyam3897/UCL) | 
| [CaSSLe](https://arxiv.org/pdf/2112.04215.pdf) | Main-training | 2022 | [Code](https://github.com/DonkeyShot21/cassle) | 
| [PFR](https://openaccess.thecvf.com/content/CVPR2022W/CLVision/papers/Gomez-Villa_Continually_Learning_Self-Supervised_Representations_With_Projected_Functional_Regularization_CVPRW_2022_paper.pdf) | Main-training | 2022 | - | 
| [SCALE](https://arxiv.org/pdf/2208.11266.pdf) | Main-training | 2022 | - | 


More details coming soon! 


