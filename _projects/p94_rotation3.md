---
layout: single
title: "C.I.T.R.O.N.S"
excerpt: My third rotation during my pre doc year
header:
  teaser: logo_citron.png
collection: project
author_profile: true
share: true
---

# Calcium Imaging Treatment using ROis; Numpy & Scipy pipeline

<p align="center">
  <img src="https://github.com/tuliofalmeida/tuliofalmeida.github.io/blob/master/images/logo_citron.png?raw=true" />
</p>

Most vertebrates exhibit early electrical activity generated by developing motor networks located in the ventral spinal cord (SC). In mice, the SC exhibits synchronized waves of electrical activity at 12 days of embryonic mice development (E12) which are essential for the proper development of the neuromuscular system. The mechanisms responsible for this Synchronized Neuronal Activity (SNA) remain unclea The main goal of my third rotation was to quantify the propagation speed of calcium waves propagating in motorneurons and other spinal cells during spontaneous calcium waves compared to calcium waves evoked after stimulation of the floorplate. The spinal cords are extracted from mice embryos at E12 from the transgenic line Isl1Cre::GCaMP6floxP, expressing the genetically encoded calcium indicator GCaMP6f specifically in the motoneurons, and from wild-type or ShhCre-GFP::Floxed-ChR2-EYFP embryos expressing the optogenetic actuator ChR2 specifically in the floor-plate. In this later condition, spinal cords were incubated with the calcium sensor Rhod2-AM to visualize calcium waves in spinal cells. Time-lapse calcium imaging was performed at 10 HZ in open-book configuration using epifluorescence microscopy. First, I was trained in spinal cord dissection and embryo slicing as well as in manipulation of the epifluorescence setup. I evoked calcium waves using electrical and light stimulation of the floorplate. To improve the analysis processes, I developed a pipeline C.I.T.R.O.N.S (Calcium Imaging Treatment using ROis; Numpy & Scipy) to perform data analysis of the calcium image data. Written in Python using procedural programming analysis techniques, this pipeline is based on the pyimagej and scijava libraries that enable the use of ImageJ functions through Python and treat the images. Also, the pipeline uses the classical high-level mathematics libraries Scipy and Numpy to calculate the metrics from the extracted signal. Therefore, the C.I.T.R.O.N.S pipeline was used to do the analysis of the current and past data collected in the lab. Pipeline workflow:

<p align="center">
  <img src="https://github.com/tuliofalmeida/tuliofalmeida.github.io/blob/master/images/citrons_horizontal.png?raw=true" />
</p>

The pipeline sped up the analysis and brought more reliability to the process, by having an GUI the user can easily choose the analysis parameters and determine the position of different ROIs. Including two main modules, one to do the image processing and the other to do the ROI analysis, the pipeline receives as input the raw image and the output is a .xlsx file with all the metrics alongside with plots, raw data, the processed images and the ROIs in the ImageJ format. All the codes are available in the [GitHub - dsco](https://github.com/tuliofalmeida/dsco) to be available for the community and future lab members. Using the pipeline was possible to reach the expected results, being better and faster than the manual analysis for all types of data. I am co-author of the publication describing how the electrical activity of the floorplate is crucial to activate motoneurons and muscles during early fetal development.

