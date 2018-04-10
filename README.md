# Browser support for WWF UK websites

WWF UK uses a tiered browser support model. This document gives details of which browsers should be supported and to what level.

This was last looked at on 10 April, using data from 1 January to 31 March 2018 on all WWF UK websites. It will be updated at the start of August  2018 using the previous quarter's information.

# Expectations

## Build to be compatible with as many browsers as possible
We build with the understanding that [websites don't have to look exactly the same in every browser](http://dowebsitesneedtolookexactlythesameineverybrowser.com), but that they should look as similar as possible.

It's worth explicitly mentioning that this covers everything on a website: HTML, CSS, and JavaScript.

We have two levels of browser support. These categories are based on what visitors are using when visiting any of WWF UK's websites.

## Level one support

Level one browsers must be fully supported.

When a site is viewed in a level one browser all content must appear and function as designed.

Slight variations in the way pages appear in different browsers are acceptable as long as it would not be obvious to a user without comparing the site in two browsers.

Example of a slight variation - the right of the two buttons below has flat colour and square corners; the left button has a gradient and rounded corners.

![](https://github.com/wwf-international/browser-support-wwf-uk/blob/master/resources/level-1-button-example.png)


Example of a variation that could use a polyfill - the `<picture>` element or `srcset`. Since `<picture>` and `srcset` degrade nicely, so if a supporter has JavaScript turned off in a browser that doesn't support these they shouldn't notice a difference.

Example of a variation that shouldn't use a polyfill - CSS Grid Layout. 60% of our visitor's browsers support grid - and, if polyfilled, then anyone with JavaScript turned off will have a degraded experience.

If in doubt with a particular case, give us a shout and we'll discuss - then add it into this document.

### Level one supported browsers

* Internet Explorer 10 and 11
* Edge 12 to latest version
* Firefox 52 to latest version
* Safari 9 to latest version
* Chrome 49 to latest version
* Safari (stock browser) on iOS 9 to latest version
* Chrome (stock browser) on Android 4.4 to latest version

For your `package.json` file, use this [Browserslist](https://github.com/ai/browserslist):

````
{
    "browserslist": [
        "explorer >= 10",
        "Edge >= 12",
        "Firefox >= 52",
        "Safari >= 9",
        "Chrome >= 49",
        "iOS >= 9",
        "ChromeAndroid >= 4.4"
    ]
}

````

## Level two support

When a site is viewed in a level two browser all text content should be viewable, all navigation and functionality should be working.

Presentation can degrade to a noticeable level, but not to the extent that functionality is lost or made materially harder to use.

### Level two supported browsers

* Internet Explorer 8 and 9
* Firefox 37 to 52
* Safari 7, 8
* Chrome 38 - 48
* Safari (stock browser) on iOS 8

## Level 3 supported browsers - unsupported

No support or testing required for these browsers.
