# Browser support for WWF UK websites

WWF UK uses a tiered browser support model. This document gives details of which browsers should be supported and to what level.

This was last looked at on 19 April, using data from 1 January to 31 March 2017 on all WWF UK websites. It will be updated at the start of July using the next quarter's information.

# Expectations

## Build to be compatible with as many browsers as possible
We build with the understanding that [websites don't have to look exactly the same in every browser](http://dowebsitesneedtolookexactlythesameineverybrowser.com), but that they should look as similar as possible.

We have two levels of browser support. These categories are based on what browser numbers we see visiting all of WWF-UK's websites.

## Level one support

Level one browsers must be fully supported.

When a site is viewed in a level one browser all content must appear and function as designed.

Slight variations in the way pages appear in different browsers are acceptable as long as it would not be obvious to a user without comparing the site in two browsers.

Example of a slight variation - the righthand of the two buttons below has flat colour and square corners; the left hand button has a gradient and rounded corners.

![](https://github.com/wwf-international/browser-support-wwf-uk/blob/master/resources/level-1-button-example.png)

Example of a variation that requires a polyfill - use of the `<picture>` element or `srcset`.

### Level one supported browsers

* Internet Explorer 10 and 11
* Edge 12 to latest version
* Firefox 31 to latest version
* Safari 6 to latest version
* Chrome 44 to latest version
* Safari (stock browser) on iOS 8, 9, and 10
* Chrome (stock browser) on Android 4.1, 5

For your `package.json` file, use this [Browserslist](https://github.com/ai/browserslist):

```
{
    "browserslist": [
        explorer >= 10, 
        Edge >= 12, 
        Firefox >= 38, 
        Safari >= 6, 
        Chrome >= 44, 
        iOS >= 8, 
        ChromeAndroid >= 4.1
    ]
}

```

## Level two support

When a site is viewed in a level two browser all text content should be viewable, all navigation and functionality should be working.

Presentation can degrade to a noticeable level, but not to the extent that functionality is lost or made materially harder to use.

### Level two supported browsers

* Internet Explorer 8 and 9
* Firefox 30 - 37
* Safari 5
* Chrome 38 - 43
* Safari (stock browser) on iOS 7

## Level 3 supported browsers - unsupported

No support or testing required for these browsers.
