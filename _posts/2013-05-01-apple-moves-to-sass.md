---
layout: post
title: Apple Store moves to Sass
---
<p class="intro">Yesterday, Apple updated their online Store with a brand new look and feel. I did some poking around in the source code and found some interesting things:</p>

## Apple Store now uses Sass

The store uses uncompressed CSS files which offers us a glimpse of the front-end technology behind the revamp. Most notably, the Apple Store now makes heavy use of Sass to pre-process its CSS files. Somewhat strangely, Apple’s developers decided to ship the uncompressed, commented CSS in the final version. An example:

    /* line 62, ../../sass/bento/_ipad.scss */
    .bento .row .tiles .ipad-l-20130410 .hero {
        position: absolute;
        top: 30px;
        left: 45px;
    }

The dates in the selector seem to indicate when the element — rather than the product itself — was created. A strange naming convention. Once rare exception is home.css which mentions both a “2012 iMac” and a “2013 iMac”. Interesting…

## What else is new?

The new store uses standard HTML5 across all pages. Other pages on Apple.com use the HTML5 doctype as well, but with the html tag’s xmlns attribute referencing the XHTML spec. The new store drops this attribute altogether.

Apple still uses images for headlines, but this time with a twist. They have developed a server-side script that generates different images based on a few parameters like size and quality.

<p class="in">The new store makes use of the Schema.org specification. Products, organizations (“Apple”) and breadcrumbs are among the types found in the source code.</p>

Find anything else? Let me know on Twitter.
