# Bootstrap 5 HTML Responsive Ecommerce Template

## Overview
 A responsive Bootstrap 5 Ecommerce template
<strong><a href="https://shima78.github.io/Bootstrap5-Ecommerce/">View Demo</a>

## Table of contents

- [Pages](#pages)
- [Demo Link](#demo-link)
- [Key Features](#key-features)
- [JSON Data](#json-data)

## Pages
The template consists of 5 pages:

* Homepage
* Category page
* Product page
* Cart page
* Checkout page

To keep code repetition to a minimum, we've used Handlebars.js as the templating engine and partials to quickly add the same code to different pages. We also use a Handlebars plugin for JSON data - this allows us to use loops and output a single HTML code block instead of repeating the same HTML.


## Demo Link
[Demo URL](https://shima78.github.io/Bootstrap5-Ecommerce/)



## Key Features

* Homepage slideshow
* Built with Bootstrap 5
* Fully responsive
* Brand logo component
* Homepage featured products slideshow component
* Category listing card showing sale badge and discount percentage
* Custom pagination component
* Header Mega menu
* Customer review component
* Company review component
* Related products slideshow component
* Custom search overlay 

## JSON Data
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



