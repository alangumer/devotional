# DEVOTIONAL
This is the repository for the devotional app, is a work in progress. Build on top of the following technologies:
* [Polymer 2](https://www.polymer-project.org/2.0/)
* [Polymer News Template](https://news-docs.polymer-project.org/)
* [Bower](https://bower.io)

## Prerequisites

### Polymer CLI

Install [polymer-cli](https://github.com/Polymer/polymer-cli):
(Need at least npm v0.3.0)

    npm install -g polymer-cli

## Setup

    git clone https://github.com/alangumer/devotional.git
    cd devotional
    bower install

## Start the development server

    dev_appserver.py .

## Build

    polymer build

## Test the build

This command serves the minified version of the app in an unbundled state, as it would be served by a push-compatible server:

    dev_appserver.py build/unbundled

This command serves the minified version of the app generated using fragment bundling:

    dev_appserver.py build/bundled

## Deploy to Google App Engine

    gcloud app deploy build/bundled/app.yaml --project [YOUR_PROJECT_ID]
