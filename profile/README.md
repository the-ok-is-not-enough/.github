# The OK Is Not Enough : A Large Scale Study of Consent Dialogs in Smartphone Applications

This org represents the state of the code used to collect the data for *The OK Is Not Enough : A Large Scale Study of Consent Dialogs in Smartphone Applications* to appear at the USENIX Security 2023. The contained repositories solely represent research artifacts and are not meant to represent the current state of the art, at least not for long. If you are interested in the current progress please contact on of the authors or check out the main repositories.

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


## How to Test/Use the Artifacts

If you want to replicate our work/use the artifacts provided to perform your own study. Follow the high level instructions below and pay close attention to the detailed information provided by the README.md of each mentioned repository.

If you only want to check if the provided code builds you can simply `cd` into the corresponding repository and run `sbt run stage` which triggers the build process and produces an executable at `<project_dir>/target/universal/stage/bin/<projectname>`. Each executable provides a `-h` flag when executed without parameter.

### Requirements (High level)

- scala 2.13
- sbt
- Java SDK
- rooted Smartphone
  - Android (we used an Galaxy A13)
  - or iOS (we used an iPhone 8s)
- Google/Apple Account
  - required to download apps 
  - required to run apps on iOS
- Apple Dev Account
  - required to run apps on iOS
