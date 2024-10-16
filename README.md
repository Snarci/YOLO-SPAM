# YOLO-SPAM: Small-Parasite-Attention-Based Model for Efficient Malaria Detection

[[`YOLO PAM PAPER`](https://www.mdpi.com/2313-433X/9/12/266)]
[[`YOLO SPAM PAPER`](https://www.sciencedirect.com/science/article/pii/S1746809424003471)]
[[`MTANET PAPER`](https://link.springer.com/chapter/10.1007/978-3-031-51026-7_6)]
[[`SAMMI PAPER`](https://iris.unica.it/handle/11584/397665)]
[[`MALARIA FRAMEWORK PAPER`](https://link.springer.com/chapter/10.1007/978-3-031-06430-2_30)]


## Setup

Before using the code, make sure to follow these setup instructions:

### [STEP 0]  Install Requirements

Install the dependencies using
```bash
pip install -r requirements.txt
```
If you are going to use GPU accelerated training feel free to remove the torch, torchvision and torchaudio rows from the requirements file and install your correct version according to [Get Started with PyTorch Locally](https://pytorch.org/get-started/locally/)

### [STEP 1]  Select Model Configuration

The full list of model configurations can be found in the "config" folder.

### [STEP 2]  Create Data Configuration

The full list of data configurations can be found in the "data" folder.

### [STEP 3]  Train a YOLO-SPAM model

A small usage example is provided in the `train_notebook.ipynb` notebook.

### Architecture Overview
<div align="center">
  <img src="https://github.com/Snarci/YOLO-SPAM/blob/main/content/SPAMv8_3H.png" width="50%" height="50%"/>
</div><br/>

### Features
* Simple to train architecture for efficient malaria detection 
* STATE-OF-THE-ART for parasite detection in [[`MP-IDB`](https://link.springer.com/chapter/10.1007/978-3-030-13835-6_7),[`IML`](https://im.itu.edu.pk/a-dataset-and-benchmark-for-malaria-life-cycle-classification-in-thin-blood-smear-images/),[`M5`](https://arxiv.org/pdf/2111.13656.pdf)]

### Visual Results
<div align="center">
  <img src="https://github.com/Snarci/YOLO-SPAM/blob/main/content/result.png" width="80%" height="80%"/>
</div><br/>

### Detection Performance Comparison

This table compares the detection performance of our proposed framework against the state-of-the-art on different datasets.

| Dataset | Species | Work | Reference Model | AP | Increase AP% |
|---------|---------|------|------------------|----|--------------|
| M5      | P. Falciparum | Sultani *et al.* (2022)~[1] | Faster R-CNN | 66.8 | - |
| M5      | P. Falciparum | Proposed Framework | YOLOv5-SPAM-3H | **71.0** | **4.2** |
| MP-IDB  | P. Falciparum | Zedda *et al.*~[2] | YOLOv5m6 | 62.5 | - |
| MP-IDB  | P. Falciparum | Proposed Framework | YOLOv5-SPAM-AH | **86.5** | **23.0** |
| MP-IDB  | P. Malariae | Zedda *et al.*~[2] | YOLOv5m6 | 80.0 | - |
| MP-IDB  | P. Malariae | Proposed Framework | YOLOv5-SPAM-AH | **94.9** | **14.9** |
| MP-IDB  | P. Ovale | Zedda *et al.*~[2] | YOLOv5m6 | 83.9 | - |
| MP-IDB  | P. Ovale | Proposed Framework | YOLOv5-SPAM-MH | **95.1** | **11.2** |
| MP-IDB  | P. Vivax | Zedda *et al.*~[2] | YOLOv5m6 | 83.1 | - |
| MP-IDB  | P. Vivax | Proposed Framework | YOLOv5-SPAM-AH | **88.3** | **5.2** |
| IML     | P. Vivax | Proposed Framework | YOLOv5-SPAM-3H | **67.4** | - |



## Contributing

Feel free to contribute by adding more papers, improving code, or providing feedback. Open issues and pull requests are welcome!

## License

This project is licensed under the [MIT License](LICENSE).

## References
[1] Sultani *et al.* (2022), [Link to Paper M5](https://arxiv.org/pdf/2111.13656.pdf)  
[2] Zedda *et al.* (ICIAP MALARIA), [Link to Paper ICIAP](https://link.springer.com/chapter/10.1007/978-3-031-06430-2_30)


## <a name="CitingYOLO-PAM and YOLO-SPAM"></a>Citing YOLO-PAM

If you use YOLO-PAM or YOLO-SPAM in your research or wish to refer to the baseline results published in the original paper, please use the following BibTeX entry.

```BibTeX
@article{YOLO_PAM,
  title       = {{YOLO}-{PAM}: {Parasite}-{Attention}-{Based} {Model} for {Efficient} {Malaria} {Detection}},
  volume      = {9},
  copyright   = {http://creativecommons.org/licenses/by/3.0/},
  issn        = {2313-433X},
  shorttitle  = {{YOLO}-{PAM}},
  url         = {https://www.mdpi.com/2313-433X/9/12/266},
  doi         = {10.3390/jimaging9120266},
  language    = {en},
  number      = {12},
  urldate     = {2023-11-30},
  journal     = {Journal of Imaging},
  author      = {Zedda, Luca and Loddo, Andrea and Di Ruberto, Cecilia},
  month       = dec,
  year        = {2023},
  note        = {Number: 12 Publisher: Multidisciplinary Digital Publishing Institute},
  keywords    = {computer vision, deep learning, early malaria diagnosis, image processing, malaria parasite detection},
  pages       = {266},
}

@article{YOLO_SPAM,
  title     = {A deep architecture based on attention mechanisms for effective end-to-end detection of early and mature malaria parasites},
  journal   = {Biomedical Signal Processing and Control},
  volume    = {94},
  pages     = {106289},
  year      = {2024},
  issn      = {1746-8094},
  doi       = {https://doi.org/10.1016/j.bspc.2024.106289},
  url       = {https://www.sciencedirect.com/science/article/pii/S1746809424003471},
  author    = {Luca Zedda and Andrea Loddo and Cecilia {Di Ruberto}},
  keywords  = {Computer vision, Deep learning, Image processing, Malaria parasites detection, Early malaria diagnosis},
}

```
## <a name="Citing our other malaria works"></a>Citing our other malaria works

If you want to cite our other malaria works in your research or wish to refer to the baseline results published in our papers, please use the following BibTeX entry.

```BibTeX
@inproceedings{zedda_sammi_2024,
	address = {Rome, Italy},
	title = {{SAMMI}: {Segment} {Anything} {Model} for {Malaria} {Identification}:},
	isbn = {978-989-758-679-8},
	shorttitle = {{SAMMI}},
	url = {https://www.scitepress.org/DigitalLibrary/Link.aspx?doi=10.5220/0012325500003660},
	doi = {10.5220/0012325500003660},
	language = {en},
	urldate = {2024-03-15},
	booktitle = {Proceedings of the 19th {International} {Joint} {Conference} on {Computer} {Vision}, {Imaging} and {Computer} {Graphics} {Theory} and {Applications}},
	publisher = {SCITEPRESS - Science and Technology Publications},
	author = {Zedda, Luca and Loddo, Andrea and Di Ruberto, Cecilia},
	year = {2024},
	pages = {367--374},
}

@incollection{zedda_mtanet_2024,
	address = {Cham},
	title = {{MTANet}: {Multi}-{Type} {Attention} {Ensemble} for {Malaria} {Parasite} {Detection}},
	volume = {14366},
	isbn = {978-3-031-51025-0 978-3-031-51026-7},
	shorttitle = {{MTANet}},
	url = {https://link.springer.com/10.1007/978-3-031-51026-7_6},
	language = {en},
	urldate = {2024-03-15},
	booktitle = {Image {Analysis} and {Processing} - {ICIAP} 2023 {Workshops}},
	publisher = {Springer Nature Switzerland},
	author = {Zedda, Luca and Loddo, Andrea and Di Ruberto, Cecilia},
	editor = {Foresti, Gian Luca and Fusiello, Andrea and Hancock, Edwin},
	year = {2024},
	doi = {10.1007/978-3-031-51026-7_6},
	note = {Series Title: Lecture Notes in Computer Science},
	pages = {59--70},
}

@incollection{zedda_deep_2022,
	address = {Cham},
	title = {A {Deep} {Learning} {Based} {Framework} for {Malaria} {Diagnosis} on {High} {Variation} {Data} {Set}},
	volume = {13232},
	isbn = {978-3-031-06429-6 978-3-031-06430-2},
	url = {https://link.springer.com/10.1007/978-3-031-06430-2_30},
	language = {en},
	urldate = {2024-03-15},
	booktitle = {Image {Analysis} and {Processing} – {ICIAP} 2022},
	publisher = {Springer International Publishing},
	author = {Zedda, Luca and Loddo, Andrea and Di Ruberto, Cecilia},
	editor = {Sclaroff, Stan and Distante, Cosimo and Leo, Marco and Farinella, Giovanni M. and Tombari, Federico},
	year = {2022},
	doi = {10.1007/978-3-031-06430-2_30},
	note = {Series Title: Lecture Notes in Computer Science},
	pages = {358--370},
}

```
