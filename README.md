# The OK Is Not Enough : A Large Scale Study of Consent Dialogs in Smartphone Applications

This org represents the state of the code used to collect the data for *The OK Is Not Enough : A Large Scale Study of Consent Dialogs in Smartphone Applications* to appear in USENIX Security 2023.


```
@inproceedings{USENIX:Koch:2023,
author = {Koch, Simon and Altpeter, Benjamin and Johns, Martin},
title = {The OK Is Not Enough : A Large Scale Study of Consent Dialogs in Smartphone Applications},
year = {2023},
booktitle = {32nd USENIX Security Symposium},
}
```

## How to Use This Org

We have multiple repositories for the different steps required to perform a mobile application analysis:

### 1. Downloading Apps

The [app-downloader](https://github.com/the-ok-is-not-enough/app-downloader) affords to download apps from the app store for both Android and iOS.


### 2. Analyzing Apps

The [scala-appanalyzer](https://github.com/the-ok-is-not-enough/scala-appanalyzer) affords to analyze a predefined set of apps against an Android (Galaxy A13 tested) or iOS (iPhone 8s tested) smartphone.

### 3. Analyzing the Results

The [scala-plotalyzer]() affords to analyze the previously collected data and to generate neat json files summarizing the relevant information for later reporting or plotting.
