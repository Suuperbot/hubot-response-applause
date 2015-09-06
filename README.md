[hubot-response](https://github.com/michaeljacobdavis/hubot-response) version of [hubot-applause](https://github.com/github/hubot-scripts/blob/master/src/scripts/applause.coffee). All credit goes to the original author [Josh French](https://github.com/joshfrench).

#### How to use
Make sure you have [hubot-response](https://github.com/michaeljacobdavis/hubot-response) installed in your hubot directory.

```
npm install --save hubot-response-applause
```

Under your responses directory, create an `applause.js` (you can name it whatever) file with

```
module.exports = [
  require('hubot-response-applause').applause,
  require('hubot-response-applause').sarcastic
];
```

#### Want to add more images?
In your `applause.js` file, just push whatever you want to the `response` array.

```
// Import the module you want
var config = require('hubot-response-applause').applause

// Extend whatever you wany
config.response.push('http://my-new-image-url-here');

// Export the altered object
module.exports = config;
```
