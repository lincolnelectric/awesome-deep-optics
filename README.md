# Awesome Deep Optics/End-to-end Optical Design

A curated list of awesome deep optics papers, inspired by [awesome-computer-vision](https://github.com/jbhuang0604/awesome-computer-vision).

Deep optics/end-to-end optical design learns optical elements simutaneously with the image processing network, with the goal to:

- find the best match between optics and network.
- encode more information from the physical world.

## Contribution

Please feel free to open pull requests or email (xinge.yang@kaust.edu.sa) to contibute to this repo.

## Courses

- Siggraph 2022. Differentiable cameras and displays. [link](https://sites.google.com/princeton.edu/neural-optics/)
- Siggraph 2020. Deep optics: joint design of optics and image recovery algorithms for domain specific cameras. [link](https://dl.acm.org/doi/abs/10.1145/3388769.3407486)
- Siggraph 2012. Computational displays: combining optical fabrication, computational processing, and perceptual tricks to build the displays of the future. [link](https://dl.acm.org/doi/abs/10.1145/2343483.2343487)

## Papers

A differentiable image formation model enables us to optimize the optics with the network. So in this part I classify papers according to the image formation model.

### 1. With wave propagation

The wave propagation model is easy to describe the perporty of diffractive elements, but less accurate for spherical/spherical lenses. Therefore, people usually optimize a single DOE or DOE with a singlet lens.

##### Diffreactive optical element (DOE)

- 2016 Encoded diffractive optics for full-spectrum computational imaging. [paper](https://www.nature.com/articles/srep33543.pdf)
- 2016 The diffractive achromat full spectrum computational imaging with diffractive optics. [paper](https://dl.acm.org/doi/pdf/10.1145/2897824.2925941), [code](https://github.com/vsitzmann/deepoptics), [slides](https://www.slideshare.net/StanfordComputationalImaging/endtoend-optimization-of-cameras-and-image-processing-siggraph-2018), [video](https://dl.acm.org/doi/10.1145/2897824.2925941).

-**2018 End-to-end optimization of optics and image processing for achromatic extended depth of field and super-resolution imaging.** [paper](https://dl.acm.org/doi/pdf/10.1145/3197517.3201333), [project](https://www.computationalimaging.org/publications/end-to-end-optimization-of-optics-and-image-processing-for-achromatic-extended-depth-of-field-and-super-resolution-imaging/), [code](https://github.com/vsitzmann/deepoptics).

- 2019 Compact Snapshot Hyperspectral Imaging with Diffracted Rotation. [paper](https://vccimaging.org/Publications/Jeon2019Hyperspectral/Jeon2019Hyperspectral.pdf), [project](https://vccimaging.org/Publications/Jeon2019Hyperspectral/)
- 2020 Learned rotationally symmetric diffractive achromat for full-spectrum computational imaging. [paper](https://opg.optica.org/optica/fulltext.cfm?uri=optica-7-10-1298&id=440114), [project](https://www.computationalimaging.org/publications/learned-rotationally-symmetric-diffractive-achromat/).
- 2021 Single-shot Hyperspectral-Depth Imaging with Learned Diffractive Optics. [paper](https://openaccess.thecvf.com/content/ICCV2021/papers/Baek_Single-Shot_Hyperspectral-Depth_Imaging_With_Learned_Diffractive_Optics_ICCV_2021_paper.pdf), [project](http://vclab.kaist.ac.kr/iccv2021/dataset.html), [video](https://www.youtube.com/watch?v=Q-9PnlkxnMs)
- 2022 Quantization-aware Deep Optics for Diffractive Snapshot Hyperspectral Imaging. [paper](https://openaccess.thecvf.com/content/CVPR2022/papers/Li_Quantization-Aware_Deep_Optics_for_Diffractive_Snapshot_Hyperspectral_Imaging_CVPR_2022_paper.pdf), [code](https://github.com/lg-li/QuantizationAwareDeepOptics)

##### DOE + Thin lens

- 2019 Deep optics for monocular depth estimation and 3D object detection. [paper](https://arxiv.org/abs/1904.08601), [project](http://www.computationalimaging.org/publications/deep-optics-depth/)
- 2020 Learning Rank-1 Diffractive Optics for Single-shot High Dynamic Range Imaging. [paper](https://vccimaging.org/Publications/Sun2020LearningRank1HDR/Sun2020LearningRank1HDR_supp.pdf), [project](https://vccimaging.org/Publications/Sun2020LearningRank1HDR/)
- 2020 End-to-end Learned, Optically Coded Super-resolution SPAD Camera. [paper](https://vccimaging.org/Publications/Sun2019SingleShotSPAD/Sun2019SingleShotSPAD.pdf), [project](https://vccimaging.org/Publications/Sun2019SingleShotSPAD/)
- 2020 Deep Optics for Single-shot High-dynamic-range Imaging. [paper](https://openaccess.thecvf.com/content_CVPR_2020/papers/Metzler_Deep_Optics_for_Single-Shot_High-Dynamic-Range_Imaging_CVPR_2020_paper.pdf), [project](https://www.computationalimaging.org/publications/deep-optics-hdr/), [code](https://github.com/computational-imaging/DeepOpticsHDR)
- 2021 Depth from Defocus with Learned Optics for Imaging and Occlusion-aware Depth Estimation. [paper](http://www.computationalimaging.org/wp-content/uploads/2021/04/DeepDfD_ICCP2021.pdf), [project](https://www.computationalimaging.org/publications/deepopticsdfd/), [code](https://github.com/computational-imaging/DepthFromDefocusWithLearnedOptics)
- 2022 Seeing Through Obstructions with Diffractive Cloaking. [paper](https://light.princeton.edu/wp-content/uploads/2022/07/seeing_through_obstructions_main.pdf), [project](https://light.princeton.edu/publication/seeing-through-obstructions/), [code](https://github.com/princeton-computational-imaging/SeeThroughObstructions)
- 2022 Hybrid diffractive optics design via hardware-in-the-loop methodology for achromatic extended-depth-of-field imaging. [paper](https://opg.optica.org/DirectPDFAccess/CC2AAA95-64FA-4A73-99FAEAA61B4A97CF_494463/oe-30-18-32633.pdf?da=1&id=494463&seq=0&mobile=no)

##### Others (Diffuser, Mask, Metasurface)

- 2020 Spectral DiffuserCam: lensless snapshot hyperspectral imaging with a spectral filter array. [paper](https://opg.optica.org/optica/fulltext.cfm?uri=optica-7-10-1298&id=440114), [code](https://github.com/Waller-Lab/SpectralDiffuserCam)
- 2021 Mask-ToF: Learning Microlens Masks for Flying Pixel Correction in Time-of-Flight Imaging. [paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Chugunov_Mask-ToF_Learning_Microlens_Masks_for_Flying_Pixel_Correction_in_Time-of-Flight_CVPR_2021_paper.pdf), [project](https://light.princeton.edu/publication/mask-tof/), [code](https://github.com/princeton-computational-imaging/MaskToF)
- 2021 Neural nano-optics for high-quality thin lens imaging. [paper](https://www.nature.com/articles/s41467-021-26443-0), [project](https://light.princeton.edu/publication/neural-nano-optics/), [code](https://github.com/Ethan-Tseng/Neural_Nano-Optics)

### 2. With ray tracing

Conventional ray tracing focuses on PSF calculations, but recent works start to directly render and optimize sensor images (differentiable ray tracing). Differential ray tracing also has some similarities to differentiable rendering.

##### Singlet Lens

- 2019 Learned large field-of-view imaging with thin-plate optics. [project](https://vccimaging.org/Publications/Peng&Sun2019LearnLargeFOV/), [video](https://dl.acm.org/doi/10.1145/3355089.3356526), [code](https://github.com/qilinsun/LearnedLargeFOV)
- 2021 End-to-end computational optics with a singlet lens for large depth-of-field imaging. [paper](https://opg.optica.org/DirectPDFAccess/D3ED35BC-DC94-4D40-B027C5426D406F5C_458026/oe-29-18-28530.pdf?da=1&id=458026&seq=0&mobile=no)
- 2021 End-to-end learned single lens design using fast differentiable ray tracing. [paper](https://opg.optica.org/view_article.cfm?gotourl=%2FDirectPDFAccess%2F8497A765%2DB6C0%2D466D%2DA8216C0290B780F2%5F462662%2Fol%2D46%2D21%2D5453%2Epdf%3Fda%3D1%26id%3D462662%26seq%3D0%26mobile%3Dno&org=King%20Abdullah%20University%20of%20Science%20and%20Technology%20)

##### Compound Lens

-**2021 End-to-end complex lens design with differentiate ray tracing.** [paper](https://vccimaging.org/Publications/Sun2021DiffLens/Sun2021DiffLens.pdf), [project](https://vccimaging.org/Publications/Sun2021DiffLens/)

- 2021 Differentiable Compound Optics and Processing Pipeline Optimization for End-To-end Camera Design. [paper](https://light.cs.princeton.edu/wp-content/uploads/2021/02/DeepCompoundOptics.pdf), [project](https://light.princeton.edu/publication/deep_compound_optics/)
- 2021 Deep learning-enabled framework for automatic lens design starting point generation. [paper](https://opg.optica.org/DirectPDFAccess/3CCFC208-3A65-4ABB-8B196EC9543FBAD5_446872/oe-29-3-3841.pdf?da=1&id=446872&seq=0&mobile=no), [project](https://lensnet.herokuapp.com/)

-**2021 dO: A differentiable engine for Deep Lens design of computational imaging systems.** [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9919421), [project](https://vccimaging.org/Publications/Wang2022DiffOptics/), [code](https://github.com/vccimaging/DiffOptics)

- 2022 Automatic Lens Design based on Differentiable Ray-tracing. [paper](https://opg.optica.org/abstract.cfm?uri=COSI-2022-CTh4C.2), [project](https://vccimaging.org/Publications/Yang2022AutoLens/), [video](https://youtu.be/8JWXvGWOG54).
- 2022 Computational Optics for Mobile Terminals in Mass Production. [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9864277)

##### Others (Sensor, Glass)

- 2021 Towards self-calibrated lens metrology by differentiable refractive deflectometry. [paper](https://opg.optica.org/DirectPDFAccess/ABF929F2-AD54-4952-8C5AC5BCD94B086C_458455/oe-29-19-30284.pdf?da=1&id=458455&seq=0&mobile=no), [project](https://vccimaging.org/Publications/Wang2021DiffDeflectometry/), [code](https://github.com/vccimaging/DiffDeflectometry)
- 2021 End-to-end sensor and neural network design using differential ray tracing. [paper](https://opg.optica.org/oe/fulltext.cfm?uri=oe-29-21-34748&id=460339)
- 2022 Adjoint Nonlinear Ray Tracing. [paper](https://dl.acm.org/doi/pdf/10.1145/3528223.3530077)

<!-- ## Talks


- [NeRF: Representing Scenes as Neural Radiance Fields for View Synthesis](https://www.youtube.com/watch?v=LCTYRqW-ne8&t=10190s), Ben Mildenhall

- [Understanding and Extending Neural Radiance Fields](https://www.youtube.com/watch?v=nRyOzHpcr4Q&feature=emb_logo&ab_channel=cvprtum), Barron et al.

- [Towards Photorealism (2nd half)](https://youtu.be/Rd0nBO6--bM?t=1992), Vladlen Koltun

- [Neural Radiance Fields for View Synthesis](https://www.youtube.com/watch?v=dPWLybp4LL0), Matthew Tancik


## Implementations


#### Tensorflow


- [NeRF](https://github.com/bmild/nerf), Mildenhall et al., 2020 | [bibtex](./NeRF-and-Beyond.bib#L168-L173)


#### PyTorch


- [NeRF-PyTorch](https://github.com/yenchenlin/nerf-pytorch), Yen-Chen Lin, 2020 | [bibtex](./citations/pytorch-nerf.txt)

- [NeRF-PyTorch-Lighting](https://github.com/kwea123/nerf_pl), [@kwea123](https://github.com/kwea123), 2020

- [NeRF-W](https://github.com/kwea123/nerf_pl/tree/nerfw), [@kwea123](https://github.com/kwea123), 2021

- [NeRF-PyTorch3D](https://github.com/facebookresearch/pytorch3d/tree/master/projects/nerf), [@facebookresearch](https://github.com/facebookresearch), 2020


#### Jax


- [JaxNeRF](https://github.com/google-research/google-research/tree/master/jaxnerf), Deng et al., 2020 | [bibtex](https://github.com/yenchenlin/awesome-NeRF/blob/main/NeRF-and-Beyond.bib#L55-L60)

- [Mip-NeRF](https://github.com/google/mipnerf), [@google](https://github.com/google), 2021 | [bibtex](./citations/mipnerf.txt) -->

## License

MI
