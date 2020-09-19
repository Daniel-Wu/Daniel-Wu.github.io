---
title: "DeepTremor"
excerpt: "Spatiotemporal earthquake projection."
header:
  image: /assets/images/tech_banner.jpg
  teaser: /assets/images/earthquake_map_ex.jpg
sidebar:
  - title: "Role"
    image: /assets/images/earthquake_map_ex.jpg
    image_alt: "logo"
    text: "Machine Learning Researcher"
  - title: "Responsibilities"
    text: "Construct deep learning models projection of earthquakes in Ridgecrest, California."
---
The occurrence of a Californian earthquake is monitored by California's Earthquake Early Warning (EEW) System, using seismograph stations located throughout the state. These stations measure the acceleration that results from an quake, which is used in numerical models to predict the shaking intensity at nearby locations in order to issue earthquake early warnings. However, these methods are slow, tend to propagate errors in initial measurements, and make assumptions about the uniformity of monitoring stations and terrain, leading to lower accuracy.

DeepTremor is a spatiotemporal generative network to achieve fast inference times while also providing accurate forecasting of earthquake progression. The model, given the magnitude of displacement recorded at different monitoring stations within a certain time window (a dense vector with location encodings), generates the predicted magnitude of displacement at future time points for each of the stations. These predictions can then be used to infer the magnitude of the shaking at locations near to the faraway stations, which can be used to determine whether a warning notification is necessary in that area.

The model was trained on roughly 36000 earthquakes that occured in Ridgecrest, California, from June to September of 2019. We achieved a percent mean absolute error of 4.2%.

![Example Earthquake Projection](/assets/images/deeptremor_ex.png)

This work was presented as a talk at the 2020 Annual Meeting of the Seismological Society of Ameria. Here's a poster we presented on our work.
<object data="/assets/posters/DeepTremor_Poster.pdf" width="1000" height="1000" type='application/pdf'/>