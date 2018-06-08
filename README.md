# dialogflow-ci
Cucumber steps for testing DialogFlow apps

## Install/run
npm install --save-dev dialogflow-ci

Run 'dialogflow-ci'

## Example project

Run 'TOKEN=<your Dialogflow token> VERSION=<v1 | v2> npm test'

## Adding/modifying steps

Add the following to a file in your cucumber load path (e.g. in features/support/load.js):
```
const cucumber = require('cucumber');
require('dialogflow-ci').steps.call(cucumber);
```

This ensures the steps are loaded into the project's Cucumber context and allow for adding and modifying steps.

## Dowloading/Uploading projects

In the dialogflow-ci project, run:
```
npm link
VERSION=v2 dialogflow-cli download <target dir> <project id>
```

