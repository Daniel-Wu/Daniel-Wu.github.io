---
title: "DeepSperm"
excerpt: "Sperm identification in testicular biopsy."
header:
  image: /assets/images/tech_banner.jpg
  teaser: /assets/images/sample_sperm.jpg
sidebar:
  - title: "Role"
    image: /assets/images/sample_sperm.jpg
    image_alt: "logo"
    text: "Machine Learning Researcher"
  - title: "Responsibilities"
    text: "Construct deep learning models for the detection of sperm in microscopy images."
---
Sperm identification and selection is an essential task when processing human testicular samples for in vitro fertilization. 
Locating and identifying sperm cells in human testicular biopsy samples is labor-intensive, time-consuming and costly.
We developed a new Computer Assisted Sperm Analysis (CASA) system which utilizes deep learning for near human-level performance 
on testicular sperm extraction (TESE), trained on a custom dataset. 
The system is to automate the identification of sperm cell(s) in testicular biopsy samples.


We collected a dataset of 702 de-identified images from IRB approved testicular biopsy samples of 30 patients.
Using a MobileNet V2 Single Shot Detector on a novel dataset of testicular biopsy sample images, we achieved an 
mAP at IOU 0.5 of 0.741 with an AR at 100 detections per image of 0.376. 
Detection rates and localization performance on sperm that has a relatively normal shape 
qualitively align with embryologist level performance. 

![Example Sperm Detection](/assets/images/sperm_model_preds.png)