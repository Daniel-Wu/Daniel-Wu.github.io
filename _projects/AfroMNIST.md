---
title: "AfroMNIST"
excerpt: "Synthetic MNIST-esque datasets for African numeral systems."
header:
  image: /assets/images/tech_banner.jpg
  teaser: /assets/images/afroMNIST.png
sidebar:
  - title: "Role"
    image: /assets/images/afroMNIST.png
    image_alt: "logo"
    text: "Data Scientist"
  - title: "Responsibilities"
    text: "Generate datasets and benchmark models on the dataset"
---

## TLDR
Afro-MNIST is a set of synthetic MNIST-style datasets for four orthographies used in Afro-Asiatic and Niger-Congo languages: Ge\`ez (Ethiopic), Vai, Osmanya, and N'Ko.
These datasets serve as drop-in replacements for MNIST. These datasets can be found [here](https://github.com/Daniel-Wu/AfroMNIST).
We hope that MNIST-style datasets will be developed for other numeral systems, and that these datasets vitalize machine learning education in underrepresented nations in the research community.

## The meat-and-bones
Classifying MNIST Hindu-Arabic numerals has become the "Hello World!" challenge of the machine learning community. This task has excited a large number of prospective machine learning scientists and has led to practical advancements in optical character recognition. 

The Hindu-Arabic numeral system is the predominant numeral system used in the world today. However, there are a sizeable number of languages whose numeric glyphs are not inherited from the Hindu-Arabic numeral system. As it relates to human language, work in machine learning and artificial intelligence focuses almost exclusively on high-resource languages such as English and Mandarin Chinese.

Unfortunately, these "mainstream" languages comprise only a tiny fraction of all extant languages. Indeed, of over 7,000 languages in the world, the vast majority are not represented in the machine learning research community. In particular, we note that there is a vast collection of alternative numeral systems for which an MNIST-style dataset is not available. 

Much of the world's linguistic diversity comes from languages spoken in developing nations. In particular, there is a wealth of linguistic diversity in the languages of Africa, many of which have dedicated orthographies and numeral systems. In this work, we focus on the Ge\`ez (Ethiopic), Vai, Osmanya, and N'Ko scripts, each of which have dedicated numerals. In particular, the Ge`ez script is used to transcribe languages such as Amharic and Tigrinya, which are spoken by some 30 million people.

Because large amounts of training data for African languages such as Amharic and Somali are not readily available, we experiment with creating synthetic numerals that mimic the likeness of handwritten numerals in their writing systems. Previous work in few-shot learning and representation learning has shown that effective neural networks can be trained on highly perturbed versions of just a single image of each class. Thus, we propose the synthetic generation of MNIST-style datasets from Unicode exemplars of each numeral. 

Starting with these unicode exemplars:
![Exemplars](/assets/images/afroMNIST_exemplars.png)

We apply a bunch of image perturbations:
![Example elastic perturbation](/assets/images/afroMNIST_perturbation.png)

and get our synthetic dataset:
![Dataset examples](/assets/images/afroMNIST.png)


which displays some interesting textual variance!
![Text features](/assets/images/afroMNIST_textfeats.png)


This project was presented at the Practical ML for Developing Countries Workshop at ICLR2020. Take a look at our [page](https://pml4dc.github.io/iclr2020/program/pml4dc_34.html), our [paper](https://pml4dc.github.io/iclr2020/papers/PML4DC2020_34.pdf) and our [slides](https://pml4dc.github.io/iclr2020/pdf/PML4DC2020_34.pdf).