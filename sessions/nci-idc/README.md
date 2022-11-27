# NCI Imaging Data Commons: Curated data and Reproducible AI workflows

## Presenters
- Andrey Fedorov, PhD ([@fedorov](https://github.com/fedorov)) - Brigham and Women's Hospital / Harvard Medical School, Boston, MA USA

## Session Date & Time
Monday, November 28, 2022
9:00 AM

## Background

**What is Imaging Data Commons (IDC)?**

![whatis](https://raw.githubusercontent.com/RSNA/AI-Deep-Learning-Lab-2022/main/sessions/nci-idc/what_is_idc.png)

* [NCI Imaging Data Commons (IDC)](https://datacommons.cancer.gov/repository/imaging-data-commons) is a cloud-based repository of publicly available cancer imaging data co-located with the analysis and exploration tools and resources 
* IDC is a node within the broader NCI Cancer Research Data Commons (CRDC) infrastructure that provides secure access to a large, comprehensive, and expanding collection of cancer research data
* IDC provides unmatched capabilities in search, visualization and subsetting of public cancer imaging, image-derived and image-related (i.e., clinical) data (45 TB and counting!): radiology and digital pathology, clinical and preclinical, images and segmentations
* Our mission is to make it easier for you to discover relevant cancer imaging data and analyze it using state of the art tools on the cloud

**Programmatic access to IDC content**

[IDC Portal](https://imaging.datacommons.cancer.gov/) is the interactive interface that allows exploring data available in IDC using a small subset of metadata attributes accompanying IDC data, visualize radiology and microscopy images and annotations, save cohorts (subsets of data) under user account based on the available metadata filters.

The real power of IDC comes, however, from programmatic interfaces available to work with IDC data. Most of the capabilities available through those interfaces and APIs are not available in the portal. As few examples, you can
* use S3 interface to download image files available in IDC (portal allows you to download a manifest, but download of files referenced from the manifest is currently not easily doable)
* use SQL interface for flexible definition of the selection filters at the level of series, studies or patients (portal exposes a very tiny set of metadata attributes, does not have the flexibility in defining filters that is needed for analysis tasks)
* combine imaging metadata with the clinical metadata in defining cohorts (portal does not expose clinical metadata available for imaging collections)

## Learning objectives

In this session you will:
* set up the (very minimal!) prerequisites to start your explorations of programmatic interfaces to IDC data
* understand the basics of IDC metadata organization
* learn how to use SQL interface to query IDC data to define subsets relevant to specific tasks
* practice how to visualize images from your cohort, download files and learn about licenses covering the data in your cohort
* identify pointers to futher learning materials that demonstate how you can develop reproducible analysis workflows using Colab applied to IDC data

## Components of the tutorial

This tutorial will leverage learning materials available in the [IDC notebooks repository](https://github.com/ImagingDataCommons/IDC-Examples/blob/master/notebooks):

1. [Setting up the prerequisites](https://github.com/ImagingDataCommons/IDC-Examples/blob/master/notebooks/getting_started/part1_prerequisites.ipynb)
2. [Basics of searching IDC data](https://github.com/ImagingDataCommons/IDC-Examples/blob/master/notebooks/getting_started/part2_searching_basics.ipynb)
3. [Working with the cohorts: visualization, download, licenses](https://github.com/ImagingDataCommons/IDC-Examples/blob/master/notebooks/getting_started/part3_exploring_cohorts.ipynb)

## Notebooks to explore on your own

* [IDC Segmentation primer: using nnU-Net for segmenting abdominal organs in chest CT](https://github.com/ImagingDataCommons/IDC-Examples/blob/master/notebooks/IDC_segmentation_primer.ipynb)
* [Introduction to exploring clinical data in IDC](https://github.com/ImagingDataCommons/IDC-Examples/blob/master/notebooks/clinical_data_intro.ipynb)

A growing number of AI models available as Colab notebooks accompanied by demonstrations of applying them to data in IDC is available in the [ModelHub.AI](http://app.modelhub.ai/) platform.

## Support and additional resources

* You can contact IDC support by sending email to support@canceridc.dev or posting your question on [IDC User forum](https://discourse.canceridc.dev).
* Please drop by IDC Office Hours to ask any questions about IDC: every Tuesday 16:30 – 17:30 (New York) and Wednesday 10:30-11:30 (New York) via Google Meet at [https://meet.google.com/xyt-vody-tvb ](https://imaging.datacommons.cancer.gov/).
* Free cloud credits are available for those who want to explore features of Google Cloud not included in the free tier (e.g., Cloud Compute Engine, Vertex AI, using Healthcare API for your data): apply [here](https://docs.google.com/forms/d/e/1FAIpQLSfXvXqficGaVEalJI3ym6rKqarmW_YUUWG6A4U8pclvR8MmRQ/viewform)

## Acknowledgments

Imaging Data Commons has been funded in whole or in part with Federal funds from the National Cancer Institute, National Institutes of Health, under Task Order No. HHSN26110071 under Contract No. HHSN261201500003l.

If you use IDC in your research, please cite the following publication:

> Fedorov, A., Longabaugh, W. J. R., Pot, D., Clunie, D. A., Pieper, S., Aerts, H. J. W. L., Homeyer, A., Lewis, R., Akbarzadeh, A., Bontempi, D., Clifford, W., Herrmann, M. D., Höfener, H., Octaviano, I., Osborne, C., Paquette, S., Petts, J., Punzo, D., Reyes, M., Schacherer, D. P., Tian, M., White, G., Ziegler, E., Shmulevich, I., Pihl, T., Wagner, U., Farahani, K. & Kikinis, R. NCI Imaging Data Commons. Cancer Res. 81, 4188–4193 (2021). http://dx.doi.org/10.1158/0008-5472.CAN-21-0950

