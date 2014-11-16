gss-starter
===========

Simple project to get you off and running with [GSS](http://gridstylesheets.org/). Built using [Yeoman](http://yeoman.io/) with some tweaks to make it work with [GSS](http://gridstylesheets.org/).

## Getting Started
1. Clone the repo.
2. `$ npm install && bower install`
3. `$ grunt serve`

[Demo](http://wl3.me/gss-starter/) can be found here. It's intentionally underwhelming.

## Why?
I created this repo because I think [GSS](http://gridstylesheets.org/) presents some really interesting possibilities for more natural layout of webapps, but found it cumbersome to get started.

This http://vimeo.com/91393694 video provides the best explanation I've seen of what [GSS](http://gridstylesheets.org/) is.

## What did you do?
This project was created using the [Yeoman Webapp Generator](https://github.com/yeoman/generator-webapp). With a few necessary modifications to make [GSS](http://gridstylesheets.org/) work.
* Installed [GSS](http://gridstylesheets.org/) using bower.
* Removed [wiredep](https://github.com/taptapship/wiredep) because it kept breaking things.
* Installed [grunt-targethtml](https://github.com/changer/grunt-targethtml) so [GSS's](http://gridstylesheets.org/) worker.js would be properly loaded.
* Added some real simple GSS constraints to the `<head>`.
```
<style type="text/gss">
  .hero-unit[width] >= 420;
  .hero-unit[height] >= 380;
  .hero-unit[center-x] == ::window[center-x];
  .hero-unit[center-y] == ::window[center-y];
</style>
```
