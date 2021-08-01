# FarmAid
![Video transcription/translation app](https://github.com/farmaid/CallForCode-FarmAid/blob/main/images/Artboard.jpg?raw=true)
FarmAid is a low code framework designed to give smallholder farmers access to critical information related to extreme weather events and crop disease outbreak.

_Read this in other languages: [English](README.md), [한국어](./docs/README.ko.md), [português](./docs/README.pt_br.md)._

## Contents

- [Submission or project name](#submission-or-project-name)
  - [Contents](#contents)
  - [Short description](#short-description)
    - [What's the problem?](#whats-the-problem)
    - [How can technology help?](#how-can-technology-help)
    - [The idea](#the-idea)
  - [Demo video](#demo-video)
  - [The architecture](#the-architecture)
  - [Long description](#long-description)
  - [Project roadmap](#project-roadmap)
  - [Getting started](#getting-started)
  - [Live demo](#live-demo)
  - [Built with](#built-with)
  - [Contributing](#contributing)
  - [Versioning](#versioning)
  - [Authors](#authors)
  - [License](#license)
  - [Acknowledgments](#acknowledgments)

## Short description

### What's the problem?

Smallholder farmers contribute around 80% of the world's food supply, yet make up a significant portion of those who live on less than $2 per day. As climate change increases the frequency and severity of extreme weather events and conditions conducive to crop-disease outbreak, smallholder farmers face significant risk to their livelihoods.

However, due to infrastructural and financial limitations, smallholder farmers are often overlooked when it comes to potential solutions that utilise artificial intelligence and machine learning.

### How can technology help?

AI and ML has the potential to act as an early warning system for smallholder farmers to take mitigating action. For example, equipped with the knowledge that therere will be damaging winds on Thursday, a farmer could harvest their crop on Tuesday. While the early harvest will have a small impact on quality due to ripenessm, this impact pales in comparison to the destruction that would have been caused by the damaging winds.

<b>The current crop disease model can predict the four most common types of crop disease (and differentiate these from a healthy leaf) with 99% accuracy.</b>

### The idea

FarmAid utilises no-code machine learning and public image datasets to train predictive models for crop disease outbreak. The final version will also combine weather data and agronomic models to create a 'Crop Damage Index'. The index can be used to alert farmers of upcoming adverse events, inform local agronomists, and provide index insurance against predicted crop damage. 

## Demo video
[![Watch the video](https://img.youtube.com/vi/UPsqNQ4bUFU/0.jpg)](https://youtu.be/UPsqNQ4bUFU)

## The architecture

The following represents the intended architecture once the platform is fully migrated to IBM Cloud in September.
The current architecture is shown in 'figure 1.2'.

![Video transcription/translation app](https://developer.ibm.com/developer/tutorials/cfc-starter-kit-speech-to-text-app-example/images/cfc-covid19-remote-education-diagram-2.png)

1. The user navigates uses the app interface to take or upload a photograph of potential crop disease.
2. Watson Speech to Text processes the audio and extracts the text.
3. Watson Translation (optionally) can translate the text to the desired language.
4. The app stores the translated text as a document within Object Storage.

## Long description

[More detail is available here](./docs/DESCRIPTION.md)

## Project roadmap

The project currently does the following things.

- Feature 1
- Feature 2
- Feature 3

It's in a free tier IBM Cloud Kubernetes cluster. In the future we plan to run on Red Hat OpenShift, for example.

See below for our proposed schedule on next steps after Call for Code 2021 submission.

![Roadmap](./images/roadmap.jpg)

## Getting started

The following code is modified from Lobe.AI (Copyright Microsoft). The model is trained with data from https://www.sciencedirect.com/science/article/pii/S2352340921004261.

In this section you add the instructions to run your project on your local machine for development and testing purposes. You can also add instructions on how to deploy the project in production.

- [sample-react-app](./sample-react-app/)
- [sample-angular-app](./sample-angular-app/)
- [Explore other projects](https://github.com/upkarlidder/ibmhacks)

## Live demo

You can find a running system to test at [callforcode.mybluemix.net](http://callforcode.mybluemix.net/).

## Built with

- [IBM Cloudant](https://cloud.ibm.com/catalog?search=cloudant#search_results) - The NoSQL database used
- [IBM Cloud Functions](https://cloud.ibm.com/catalog?search=cloud%20functions#search_results) - The compute platform for handing logic
- [IBM API Connect](https://cloud.ibm.com/catalog?search=api%20connect#search_results) - The web framework used
- [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
- [Maven](https://maven.apache.org/) - Dependency management
- [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags).

## Authors

<a href="https://github.com/Call-for-Code/Project-Sample/graphs/contributors">
  <img src="https://contributors-img.web.app/image?repo=Call-for-Code/Project-Sample" />
</a>

- **Billie Thompson** - _Initial work_ - [PurpleBooth](https://github.com/PurpleBooth)

## License

This project is licensed under the Apache 2 License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Based on [Billie Thompson's README template](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2).
