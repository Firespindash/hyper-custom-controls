# hyper-custom-controls-minimalist

> A minimalist version of the hyper-custom-controls by @guilhermerodz

It does autohide titlebar and hamburger menu by default, but it is not configurable yet.
To install clone this repo in `~/.hyper-plugins/local/`  and add `hyper-custom-controls-minimalist` to the localPlugins in the `~/.hyper.js` file, then reload hyper going to `View -> Full Reload` or pressing `Cmd + Shift + R`.
For now it can only be installed locally, instead of being installed from npm.

> Add Mac-like controls to Hyper Terminal, but highly customizable

*A screenshot taken in KDE linux environment* \
![The visual approach](https://raw.githubusercontent.com/Firespindash/hyper-custom-controls-minimalist/master/media/result.png)

## Configuration

In your `~/.hyper.js`, you can configure settings for `hyper-custom-controls`.

```js
modules.exports = {
  config: {
    // NOTE: All properties below are optional and have a default value.
    hyperCustomControls: {
      side: 'left', // Default: 'left'
      circleSize: 11, // Default: 11
      circleGap: 7.5, // Default: 7.5
      distanceToSide: 15, // Default: 15
      opacity: 1, // Default: 1
      hoverOpacity: 0.5, // Default: 0.5

      // Default controls below:
      // NOTE: You can remove a control, if you want to.
      controls: [
        {
          type: 'close',
          color: '#F24F55',
        },
        {
          type: 'minimize',
          color: '#FBC536',
        },
        {
          type: 'maximize',
          color: '#39EA48',
        },
      ],
    },
  },
};
```
