# speech-synth

> Simple text to speech module built on Web Speech API.

- Try out a live demo of the component [here](https://speech-synth.herokuapp.com)

- The NPM page can be found [here](https://www.npmjs.com/package/speech-synth)

- The GitHub page can be found [here](https://github.com/CaribouBlue/speech-synth)

## Table of Contents

1. [Usage](#usage)
  1. [Initial Setup](#initial-setup)
  1. [Component API](#component-api)
1. [Team](#team)

## Usage

### Install Module

run ```npm install speech-synth --save``` in console while in root directory to add the component to your project.

### Initial Setup

Import the module buy using a requrie statement:
```const speech = require('speech-synth');```

or an import statement:
```import speech from 'speech-synth';```

### Component API

- __say__:
  - Description: convert text to speech
  - Type: Method
  - Params: (input, voiceURI)
    - input -> String to be spoken
    - voiceURI -> name of the voice to use
      - Default: ```'Google US English'```
  - Return: none
```
  speech.say('hello')
```

- __getVoiceNames__:
  - Description: returns an array of all voiceURI options that can be used with the say method
  - Type: Method
  - Params: none
  - Return: Array[String]
```
  speech.getVoiceNames()
```

__Example__:
```
  let voice = speech.getVoiceNames()[3];
  speech.say('My voice is Google Deutsch', voice);
```

## Team

  - __Development Team Members__: 
    - Alec Draymore