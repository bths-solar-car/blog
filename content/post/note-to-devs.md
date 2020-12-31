+++
title = "Guide for Blogging (devs only)"
date = "2020-09-11T13:24:16-05:00"
author = "THE SYSTEM ADMIN"
authorTwitter = "" #do not include @
cover = ""
tags = ["SYSTEM ADMIN"]
keywords = ["", ""]
summary = "This post will teach you everything you need to know making posts on this blog. Read thoroughly and with caution. Experience with Git and GitHub is a must here."
+++

## Intro

This post will describe the ins and outs of markdown files and hugo. Use with caution and with sincerity. A good developer knows what problems may arise. It is up to you to decide what to do, but be wary of anything you don't understand. Spaghetti code is frowned upon and should only be used if you fully understand the code.

You may notice that the rest of this post is gibberish, don't worry. This is intended to show what features are available to you. **If you want a certain look in one of your posts, look into the markdown.**

You will find many similarities between mediums that utilize markdown like Discord. In Discord, you use '>' to represent a quote. You can also use this same character in markdown.

### Very Important!
When making a new post, assuming you have `hugo` installed...

#### If you don't have hugo installed...
See Hugo's quickstart guide [here](https://gohugo.io/getting-started/quick-start/).

*Ignore step 2 and step 3, we've already created the blog and the theme.*

#### Moving on...
At the *beginning* of every post, there is a configuration space where you can set the title, date, author and description of the post.

There are _two_ ways of writing this configuration. They're both very simple, and it doesn't matter which way you set up the configuration, as long as it's consistent in the current post.

##### First Way

```markdown
+++
title = ""
date = "2020-12-30"
author = ""
tags = ["", ""]
keywords = ["", ""]
summary = ""
+++
```
Notice how this uses `+++` and `=` characters.

##### Second Way

```markdown
---
title: ""
date: "2020-12-30"
author: ""
tags: ["", ""]
keywords: ["", ""]
summary: ""
---
```
Notice how this uses `---` and `:` characters.

### Header Level 3

The header up above is written exactly as follows: `### Header Level 3`.

The code snippet below is exactly as follows: back ticks are used to indicate code snippets.

```css
/* This code snippet can be used to show algorithms relevant to Project BlueBird */
/* PostCSS code */

pre {
  background: #1a1a1d;
  padding: 20px;
  border-radius: 8px;
  font-size: 1rem;
  overflow: auto;

  @media (--phone) {
    white-space: pre-wrap;
    word-wrap: break-word;
  }

  code {
    background: none !important;
    color: #ccc;
    padding: 0;
    font-size: inherit;
  }
}
```

```js
// Features a diverse variety of languages
// JS code

const menuTrigger = document.querySelector('.menu-trigger')
const menu = document.querySelector('.menu')
const mobileQuery = getComputedStyle(document.body).getPropertyValue('--phoneWidth')
const isMobile = () => window.matchMedia(mobileQuery).matches
const isMobileMenu = () => {
  menuTrigger.classList.toggle('hidden', !isMobile())
  menu.classList.toggle('hidden', isMobile())
}

isMobileMenu()

menuTrigger.addEventListener('click', () => menu.classList.toggle('hidden'))

window.addEventListener('resize', isMobileMenu)
```

```html
<!-- Comments work too -->
<!-- HTML code -->

<section id="main">
  <div>
   <h1 id="title">{{ .Title }}</h1>
    {{ range .Pages }}
      {{ .Render "summary"}}
    {{ end }}
  </div>
</section>
```

#### Header Level 4

The header up above is written exactly as follows: `#### Header Level 4`.

Note that the number of # corresponds to the header's level/size.

Below, you'll find that bullet points and even dash-points work in levels of indentation.

- Item 1
- Item 2
- Item 3
- Item 4
    - Item 4a
    - Item 4b
* Here, I'm using asterisks, but it is formatted the same as dashes.
* Same thing here
    * Same thing here as well
1. Numbered item 1
2. Numbered item 2
3. Numbered item 3
4. Numbered item 4
    - indented items work too.

Aliquam erat volutpat. In hac habitasse platea dictumst. Nunc ut tincidunt mauris. Sed at gravida risus, id semper magna. Nullam vitae enim mattis, sodales neque non, pharetra elit. Cras sit amet sagittis augue, et finibus turpis. Ut tempus tincidunt diam vel pharetra. Nulla porttitor odio sit amet nulla scelerisque, quis aliquam mi imperdiet. Sed tincidunt dui vel tellus vestibulum rhoncus. Donec tempus ultrices velit.

