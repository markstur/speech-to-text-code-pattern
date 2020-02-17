<h1 align="center" style="border-bottom: none;">Speech to Text Code Pattern 🗣</h1>
<h3 align="center">Sample React app for playing around with the Watson Speech to Text service.</h3>
<p align="center">
  <a href="http://travis-ci.org/watson-developer-cloud/speech-to-text-code-pattern">
    <img alt="Travis" src="https://travis-ci.org/watson-developer-cloud/speech-to-text-code-pattern.svg?branch=master">
  </a>
  <a href="#badge">
    <img alt="semantic-release" src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg">
  </a>
</p>
</p>

✨ **Demo:** https://speech-to-text-code-pattern.ng.bluemix.net/ ✨

## Flow

<p align="center">
  <img alt="architecture" width="600" src="./public/architecture.png">
</p>

1. User supplies an audio input to the application (running locally, in the IBM Cloud or in IBM Cloud Pak for Data).
1. The application sends the audio data to the Watson Speech to Text service through a [WebSocket connection](https://cloud.ibm.com/docs/services/speech-to-text?topic=speech-to-text-websockets).
1. As the data is processed, the Speech to Text service returns information about extracted text and other metadata to the application to display.

## Deployment options

Click on one of the options below for instructions on deploying the Node.js server.

|   |   |   |   |
| - | - | - | - |
| [![local](https://raw.githubusercontent.com/IBM/pattern-utils/master/deploy-buttons/local.png)](doc/source/local.md) | [![openshift](https://raw.githubusercontent.com/IBM/pattern-utils/master/deploy-buttons/openshift.png)](doc/source/openshift.md) | [![cf](https://raw.githubusercontent.com/IBM/pattern-utils/master/deploy-buttons/cf.png)](doc/source/cf.md) |

## Using the web app

### TODO: Explain/show what it does

> Need more information? See the [authentication wiki](https://github.com/IBM/node-sdk-core/blob/master/AUTHENTICATION.md).

## Tests

#### Unit tests

Run unit tests with:

```
npm run test:components
```

See the output for more info.

#### Integration tests

First you have to make sure your code is built:

```
npm run build
```

Then run integration tests with:

```
npm run test:integration
```

## Directory structure

```none
.
├── app.js                      // Express routes
├── config                      // Express configuration
│   ├── error-handler.js
│   ├── express.js
│   └── security.js
├── package.json
├── public                      // Static resources
├── server.js                   // Entry point
├── test                        // Tests
└── src                         // React client
    └── index.js                // App entry point
```

## License

This sample code is licensed under the [MIT License](https://opensource.org/licenses/MIT).

## Open Source @ IBM

Find more open source projects on the [IBM Github Page](http://ibm.github.io/)
