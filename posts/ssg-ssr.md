---
title: 'When to use Static Generation v.s. Server-side Rendering'
date: '2020-09-07'
---

We recommend using **Static Generation** (with and without data) whenever possible because your page can be built once and served by CDN, wich makes it much faster than having a server render the page on every request.

You can use Static Generation for many types of page, including:

- Marketing pages
- Blog posts
- E-commerce product listings
- Help and documentation

You should ask yourself: "Can i pre-render this page **ahead** of a user's request?" If the answer is yes, the you should choose Static Generation.

On the other hand, Static generation is **not** a good idea if you cannot pre-render a page ahead of a user's request. Maybe your page shows frequently updated data, and the page content changes on very request.

In this case, you can use **Server-Side Rendering**. It will be slower, but the pre-rendered page will always be up-to-date. Or you can skip pre-rendering and use client-side JavaScript to populate data.