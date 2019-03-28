# Introduction
This is an unofficial repository that is used to run [LanguageTool](https://www.languagetool.org/) in Docker.

LanguageTool is an Open Source proofreading software for English, French, German, Polish, Russian, and [more than 20 other languages](https://languagetool.org/languages/). It finds many errors that a simple spell checker cannot detect.

# Usage

## Using Docker Hub
```
docker pull erikvl87/languagetool
docker run --rm -p 8010:8010 erikvl87/languagetool
```

This will pull the `latest` tag from Docker Hub. Optionally, [pull a tag](https://hub.docker.com/r/erikvl87/languagetool/tags) to pin onto a fixed version. These versions are derived from the official LanguageTool releases.

## Using the Dockerfile
```
git clone https://github.com/Erikvl87/docker-languagetool.git
docker build -t languagetool .
docker run --rm -it -p 8010:8010 languagetool
```
