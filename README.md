# FarmAid
![Video transcription/translation app](https://github.com/farmaid/CallForCode-FarmAid/blob/main/images/Artboard.jpg?raw=true)
FarmAid is a low code framework designed to give smallholder farmers access to critical information related to extreme weather events and crop disease outbreak.

_Read this in other languages: [English](README.md), [한국어](./docs/README.ko.md), [português](./docs/README.pt_br.md)._

## Short description

### What's the problem?

Smallholder farmers contribute around 80% of the world's food supply, yet make up a significant portion of those who live on less than $2 per day. As climate change increases the frequency and severity of extreme weather events and conditions conducive to crop-disease outbreak, smallholder farmers face significant risk to their livelihoods.

However, due to infrastructural and financial limitations, smallholder farmers are often overlooked when it comes to potential solutions that utilise artificial intelligence and machine learning.

### How can technology help?

AI and ML has the potential to act as an early warning system for smallholder farmers to take mitigating action. For example, equipped with the knowledge that there will be damaging winds on Thursday, a farmer could harvest their crop on Tuesday. While the early harvest may have a small impact on quality due to under-ripeness, this impact pales in comparison to the destruction that would have been caused by the damaging winds.

<b>The current crop disease model can predict the four most common types of crop disease (and differentiate these from a healthy leaf) with 99% accuracy.</b>

### The idea

FarmAid utilises no-code machine learning and public image datasets to train predictive models for crop disease outbreak. The final version will also combine weather data and agronomic models to create a 'Crop Damage Index'. The index can be used to alert farmers of upcoming adverse events, inform local agronomists, and provide index insurance against predicted crop damage. 

## Demo video
[![Watch the video](https://img.youtube.com/vi/UPsqNQ4bUFU/0.jpg)](https://youtu.be/UPsqNQ4bUFU)

## The architecture

The following represents the intended architecture once the platform is fully migrated to IBM Cloud in September.

![Video transcription/translation app](https://github.com/farmaid/CallForCode-FarmAid/blob/main/images/IBMSUBMISSIONDIAGRAM.png?raw=true)

1. The user navigates uses the app interface to take or upload a photograph of potential crop disease.
2. The TensorFlow model via Docker with Flask framework detects the presence of crop disease.
3. Watson Assistant takes input from internal and external databases to provide details specific to the context of the user.
4. The user receives push notifications when relevant information is received by the cloud infrastructure.

## Long description

[More detail is available here](./docs/DESCRIPTION.md)

## Project roadmap

The project currently does the following things.

- Allows users to sign up and onboard
- Receive accurate hyperlocal weather information and push notifications in case of extreme weather event alert
- Send images of potential crop disease for analysis against model trained to detect the four most common types of disease with 99% accuracy.

See below for our proposed schedule on next steps after Call for Code 2021 submission.

![Roadmap](https://github.com/farmaid/CallForCode-FarmAid/blob/main/images/IBM%20Timeline.png?raw=true)

## Getting started

The model is trained with data from https://www.sciencedirect.com/science/article/pii/S2352340921004261.

- Follow instructions from https://github.com/lobe/flask-server#readme
- Instead of using files from the above repository, download from 'Model' in this repository
- Deploy Flask app to IBM Cloud: https://github.com/IBM/python-flask-app
- Clone Adalo app https://previewer.adalo.com/37d703b5-0b11-4880-abeb-ccf7fdb1e9f8
- Connect app to IBM Cloud: https://help.adalo.com/integrations/custom-actions

## Built with

- [IBM Cloud Pak® for Data](https://www.ibm.com/au-en/cloud/paks/) - Used for cloud functions
- [ADALO](https://www.adalo.com/) - Used to build app interface
- [LOBE](https://www.lobe.ai/) - Used to build ML model

## License

This project is licensed under the Apache 2 License - see the [LICENSE](LICENSE) file for details.

## Acklowedgments

For the purposes of creating an MVP, LOBE.AI was used to create the ML model. The code provided in this repo is thanks to Lobe.


