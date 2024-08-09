# YOLO-SPAM: Small-Parasite-Attention-Based Model for Efficient Malaria Detection
<!---
[[`Paper`](https://www.mdpi.com/2313-433X/9/12/266)]
--->
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


## Setup

Before using the code, make sure to follow these setup instructions:

### [STEP 1] Ultralytics Installation

Extract the "ultralytics" zip file and place it in your Python packages folder.

### [STEP 2]  Select Model Configuration

The full list of model configurations can be found in the "config" folder.

### [STEP 3]  Create Data Configuration

The full list of data configurations can be found in the "data" folder.

### [STEP 4]  Train a YOLO-SPAM model

A small usage example is provided in the `train_notebook.ipynb` notebook.

## Contributing

Feel free to contribute by adding more papers, improving code, or providing feedback. Open issues and pull requests are welcome!

## License

This project is licensed under the [MIT License](LICENSE).

## References
[1] Sultani *et al.* (2022), [Link to Paper M5](https://arxiv.org/pdf/2111.13656.pdf)  
[2] Zedda *et al.* (ICIAP MALARIA), [Link to Paper ICIAP](https://link.springer.com/chapter/10.1007/978-3-031-06430-2_30)

<!---
## <a name="CitingYOLO-PAM"></a>Citing YOLO-PAM

If you use YOLO-PAM in your research or wish to refer to the baseline results published in the original paper, please use the following BibTeX entry.

```BibTeX
@article{zedda_yolo-pam_2023,
	title = {{YOLO}-{PAM}: {Parasite}-{Attention}-{Based} {Model} for {Efficient} {Malaria} {Detection}},
	volume = {9},
	copyright = {http://creativecommons.org/licenses/by/3.0/},
	issn = {2313-433X},
	shorttitle = {{YOLO}-{PAM}},
	url = {https://www.mdpi.com/2313-433X/9/12/266},
	doi = {10.3390/jimaging9120266},
	language = {en},
	number = {12},
	urldate = {2023-11-30},
	journal = {Journal of Imaging},
	author = {Zedda, Luca and Loddo, Andrea and Di Ruberto, Cecilia},
	month = dec,
	year = {2023},
	note = {Number: 12
  Publisher: Multidisciplinary Digital Publishing Institute},
	keywords = {computer vision, deep learning, early malaria diagnosis, image processing, malaria parasite detection},
	pages = {266},
}
```
--->

