svg-transform-parser2
====================

Parse SVG transform in Javascript

> Forked from [nidu/svg-transform-parser](https://github.com/nidu/svg-transform-parser), support multiple rules with same name.

## Installation

    npm install svg-transform-parser2

## Usage

    var parseSvgTransform = require('svg-transform-parser2').parse;

    parseSvgTransform("translate(10,20) translate(2 0.5)");
    // [
    //     {
    //         "key": "translate",
    //         "value": {
    //             "tx": 10,
    //             "ty": 20
    //         }
    //     },
    //     {
    //         "key": "translate",
    //         "value": {
    //             "tx": 2,
    //             "ty": 0.5
    //         }
    //     }
    // ]


## Compile pegjs

    npm run-script compile

## Tests
  
    npm test