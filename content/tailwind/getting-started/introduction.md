---
layout: home
title: Flowbite - Tailwind CSS component library
description: Get started with the most popular open-source library of interactive UI components built with the utility classes from Tailwind CSS
group: getting-started
toc: true
cleanTitle: true

next: Quickstart
nextLink: golang/getting-started/quickstart/
---

## Introduction

Flowbite is an open-source library of UI components based on the utility-first Tailwind CSS framework featuring dark mode support, a Figma design system, and more.

It includes all of the commonly used components that a website requires, such as buttons, dropdowns, navigation bars, modals, but also some more advanced interactive elements such as datepickers.

All of the elements are built using the utility classes from Tailwind CSS and vanilla JavaScript.

<iframe width="100%" class="my-8 rounded-lg shadow-lg yt-video" src="https://www.youtube.com/embed/KaLxCiilHns" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Here's a quick overview of the Flowbite ecosystem including the open source Tailwind components library, the Figma design files, and the pro version.

<div class="mt-10 lg:grid lg:grid-cols-2 lg:gap-8">
    <a href="{{< ref "tailwind/getting-started/quickstart" >}}" class="block p-6 mb-6 bg-white rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:hover:bg-gray-700 hover:bg-gray-100 dark:border-gray-700 lg:mb-0">
        <h3 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Quickstart</h3>
        <p class="font-normal text-gray-700 dark:text-gray-400">Learn how to get started by downloading and configuring Flowbite locally on your machine and start developing.</p>
    </a>
    <a href="{{< ref "tailwind/components/alerts" >}}" class="block p-6 mb-6 bg-white rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:hover:bg-gray-700 hover:bg-gray-100 dark:border-gray-700 lg:mb-0">
        <h3 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Components</h3>
        <p class="font-normal text-gray-700 dark:text-gray-400">Explore the Tailwind CSS elements such as buttons, navbars, alerts, dropdowns and use them to build your website.</p>
    </a>
    <a href="{{< param homepage >}}/figma/" class="block p-6 mb-6 bg-white rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:hover:bg-gray-700 hover:bg-gray-100 dark:border-gray-700 lg:mb-0">
        <h3 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Figma design files</h3>
        <p class="font-normal text-gray-700 dark:text-gray-400">Prototype and design your website before coding with the Flowbite Figma file which is based on the Tailwind CSS classes.</p>
    </a>
    <a href="{{< param homepage >}}/pro/" class="block p-6 mb-6 bg-white rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:hover:bg-gray-700 hover:bg-gray-100 dark:border-gray-700 lg:mb-0">
        <h3 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Upgrade to Pro</h3>
        <p class="font-normal text-gray-700 dark:text-gray-400">Take your Figma and Tailwind CSS development to the next level with thousands more elements and pages with Flowbite Pro.</p>
    </a>
</div>

## Using Flowbite

One of the disadvantages of Tailwind CSS compared to other frameworks is that it doesn't have a base set of components. This makes it really hard to quickly prototype a user interface.

This is where Flowbite comes into play: it's basically Tailwind CSS, but you get all of the components that you would normally get with a classic CSS framework like Bootstrap or Bulma.

There are 52 types of UI components including buttons, alerts, breadcrumbs, pagination, and navbars. Flowbite also includes some custom JavaScript that enables interactive components, such as dropdowns, modals, tooltips, and many more.

## Getting started

Flowbite is technically a plugin that can be included into any existing Tailwind CSS project. To get started, you first need to make sure that you have a working Tailwind CSS project installed and that you also have Node and NPM installed on your machine.

### Require via NPM

1. Install the latest version of Flowbite using NPM:

```bash
npm i flowbite
```

2. Include Flowbite as a plugin inside the `tailwind.config.js` file:

```javascript
module.exports = {
  plugins: [require("flowbite/plugin")],
};
```

3. Require the JavaScript code that powers the interactive elements before the end of your `<body>` tag:

```html
<script src="../path/to/flowbite/dist/flowbite.js"></script>
```

4. Additionally to your own `content` data you should add `flowbite` to apply the classes from the interactive elements in the `tailwind.config.js` file:

```javascript
module.exports = {
  content: ["./node_modules/flowbite/**/*.js"],
};
```

If you use Webpack or other bundlers you can also import it like this:

```javascript
import "flowbite";
```

### Include via CDN

If you want to quickly test out Flowbite you can easily include the following CSS and JavaScript files.

Require the following minified stylesheet inside the `head` tag:

```html
<link rel="stylesheet" href="https://unpkg.com/flowbite@{{< current_version >}}/dist/flowbite.min.css" />
```

And include the following javascript file before the end of the `body` element:

```html
<script src="https://unpkg.com/flowbite@{{< current_version >}}/dist/flowbite.js"></script>
```

Please remember that the best way to work with Tailwind CSS and Flowbite is by purging the CSS classes.

## Tailwind CSS 2.0

Flowbite is fully compatible with the 2.x versions of Tailwind CSS.

## Tailwind CSS 3.0

Feel free to upgrade to version 3 of Tailwind CSS as there are no breaking changes when using the components from Flowbite.

## Figma

The components from Flowbite are first conceptualized and designed in Figma using the latest features such as variants, auto-layout, grids, responsive layouts, and more.

Learn more by checking out <a href="{{< param homepage >}}/figma/">Flowbite's Figma design system</a> and start designing your Tailwind CSS projects before actually coding them.

<div class="mt-8 -mb-5">
  {{< requires_nextjs >}}
</div>

## Next.js

If you're using React as a front-end library and Next.js as a framework you can also use the components from Flowbite React such as the modals, dropdowns, and navbars to speed up your development time coupled with the utility classes from Tailwind CSS.

Learn how to <a href="{{< ref "tailwind/getting-started/next-js" >}}">install Tailwind CSS and Flowbite with Next.js and React</a>.
