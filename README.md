# Browser support for WWF UK websites

WWF UK uses a tiered browser support model. This document gives details of which browsers should be supported and to what level.

# Expectations #

## Build to be compatible with as many browsers as possible ##
We build with the understanding that [websites don't have to look exactly the same in every browser](http://dowebsitesneedtolookexactlythesameineverybrowser.com), but that they should look as similar as possible.

We have two levels of browser support. These categories are based on what browser numbers we see visiting all of WWF-UK's websites.

## Level one support

Level one browsers must be fully supported.

When a site is viewed in a level one browser all content must appear and function as designed.

Slight variations in the way pages appear in different browsers are acceptable as long as it would not be obvious to a user without comparing the site in two browsers.

Example of a slight variation - on  the right is a button viewed in IE8 which doesn't support CSS gradients and rounded corners, so it has flat colour and square corners.

![](https://github.com/wwf-international/browser-support-wwf-uk/blob/master/resources/level-1-button-example.png)


Example of a variation that requires a polyfill - use of the `<picture>` element or `srcset`.

### Level one supported browsers

* IE 9, 10, 11
* Edge
* Firefox 31 - latest evergreen version
* Safari 6+
* Chrome 38 - latest evergreen version
* Safari (stock browser) on iOS 7, 8, 9
* Chrome (stock browser) on Android 4.1, 5

## Level two support

When a site is viewed in a level two browser all text content should be viewable, all navigation and functionality should be working.

Presentation can degrade to a noticeable level, but not to the extent that functionality is lost or made materially harder to use.

Components of a site may omit support for level two browsers if they are not essential. In this case a message should be displayed, stating that a more recent browser is required.

Example: The energy quiz is not essential to the Earth Hour site.  A message is displayed explaining that the quiz doesn't work with older browsers.

![](https://github.com/wwf-international/browser-support-wwf-uk/blob/master/resources/level-2-earth-hour-quiz-example.png)


### Level two supported browsers

* IE  8
* Firefox 3 - 30
* Safari 5
* Chrome 25 - 37

## Level 3 supported browsers - unsupported

No support or testing required for these browsers.
