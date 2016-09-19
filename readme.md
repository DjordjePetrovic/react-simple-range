# react-simple-range

[![npm version](https://badge.fury.io/js/react-simple-range.svg)](https://badge.fury.io/js/react-simple-range)

A simple React component for inputting a number between a min and a max value using a slider.

_nb: this package is in development and getting daily updates - production use not recommended while this message exists!_

## Install

```npm install react-simple-range --save```

## Usage

Import React and this component using your chosen module bundler:

```
import React from 'react';
import ReactDOM from 'react-dom';
import ReactSimpleRange from 'react-simple-range';
const rootElement = document.getElementById('app');

ReactDOM.render(<ReactSimpleRange />, rootElement);
```

Or the pre-minified version:
```
import ReactSimpleRange from 'react-simple-range/lib/index-min';
```

## Props

Name | Type | Default | Description
---|---|---|---|---
min | number | `0` | Minimum slider value
max | number | `100` | Maximum slider value
step | number | `1`  | Number inc/decremented when slider value is changed. The range of the slider (max - min) should be evenly divisible by this
onChange | function | [NOOP](https://en.wikipedia.org/wiki/NOP) | Function to be called when the slider value changes
value | number | `props.defaultValue` | Set current value of slider
defaultValue | number | `0` | Set initial value of slider
className | string | `undefined` | Additional CSS class to be apply to root div if required
sliderHeight | string | `'6px'` | Height of slider
sliderColor | string | `'#9E9E9E'` | Color of slider
trackColor | string | `'#03A9F4'` | Color of track indicating progress
thumbHeight | string | `'8px'` | Height (and width currently) of thumb
thumbColor | string | `'#fff'` | Color of thumb
thumbOffsetTop | string | `'-2px'` | Top property to apply to thumb
thumbOffsetLeft | string | `'-5px'` | Margin-left property to apply to thumb

## Development

Clone the repo then run ```npm start``` in the cloned directory to start webpack-dev-server and serve the examples.

## Commands

Name | Effect
:---|:---
`npm start` | Starts a webpack-dev-server, currently serves the `examples/` directory to `http://localhost:8080/`
`npm run test` | No effect for now - tests being added IMMINENTLY

## Future additions

- Slider orientation
- Better perf
- Other stuff