#  Bootstrap 5 HTML Responsive Ecommerce Template

## Overview
For the fashion focused online store, this template is a responsive Bootstrap 5 Ecommerce template with a "Ken Burns" effect on the homepage slideshow, angled banners, and a custom image hotspot banner with popout product cards. Large product images on category pages give you ample room for showcasing products while simultaneously providing easy navigation throughout the website. It's the perfect starting point for any fashion retail website, and the template's clean and minimal design means it's easy to modify and painless to integrate with your custom Ecommerce application. And above all, it's free.

<strong><a href="https://alpine-html-bootstrap.vercel.app/">View Demo</a> | <a href="https://github.com/shima78/Bootstrap5-Ecommerce/archive/refs/heads/main.zip">Download ZIP</a></strong>

![Bootstrap 5 Responsive HTML Fashion Store Template](https://pixelrocket-public-assets.s3.eu-west-2.amazonaws.com/github-assets/alpine-html/homepage-medium.jpg "Alpine | Responsive Bootstrap 5 Ecommerce Template")

## Table of contents

- [Template Pages](#template-pages)
- [Demo Link](#demo-link)
- [Template Key Features](#template-key-features)
- [Template JSON Data](#template-json-data)



## Template Pages
The template consists of 5 pages:

* Homepage
* Category page
* Product page
* Cart page
* Checkout page

To keep code repetition to a minimum, we've used Handlebars.js as the templating engine and partials to quickly add the same code to different pages. We also use a Handlebars plugin for JSON data - this allows us to use loops and output a single HTML code block instead of repeating the same HTML.


## Demo Link
[Demo URL](https://alpine-html-bootstrap.vercel.app/)


## Template Key Features

* Homepage slideshow (using Swiper.js)
* Built with Bootstrap 5
* Fully responsive
* Brand logo component
* Homepage featured products slideshow component (using Swiper.js)
* Image Hotspot component with popout product card (using Tippy.js)
* Instagram slideshow component
* Category listing card showing sale badge and discount percentage
* Custom pagination component
* Header Megamenu
* Customer review component
* Company review component
* Related products slideshow component
* Offcanvas category filter display
* Header cart offcanvas display
* Custom search overlay


## Template JSON Data
The Webpack Handlebars plugin that we use comes with a very handy utility that allows us to pass in JSON files as template data.

Please navigate to: src/data. Here is where our template data JSON files reside. You can edit, remove or add your own to this folder.

Again, if we reference our category page loop:

```
{{#if (config category-products)}}
    {{#each (limit category-products.entries 4)}}
        <div class="col-12 col-sm-6 col-md-4">
            {{> listing-cards/listing-card this }}
        </div>
    {{/each}}
{{/if}}
```

The important part here with regards to template data is category-products.entries. What this means is that inside our data folder you will find a JSON file called "category-products". This category-products.json file has a "key" called "entries".


