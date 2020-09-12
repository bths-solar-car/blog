+++
title = "Dear Future Developers of Project BlueBird..."
date = "2020-09-11"
author = "THE SYSTEM ADMIN"
authorTwitter = "" #do not include @
cover = ""
tags = ["", ""]
keywords = ["", ""]
description = "This post will teach you everything you need to know making posts on this blog. Read thoroughly and with caution. Experience with Git and GitHub is a must. **Work In Progress**"
+++

## Intro

This post will describe the ins and outs of markdown files and hugo. Use with caution and with sincerity. A good developer knows what problems may arise. It is up to you to decide what to do, but be wary of anything you don't understand. Spaghetti code is frowned upon and should only be used if you fully understand the code.

You may notice that the rest of this post is gibberish, don't worry. This is intended to show what features are available to you. **If you want a certain look in one of your posts, look into the markdown.**

Like in Discord and in Markdwon, you can use '>' to represent a quote from a person or passage in another text.

### Very Important!
When making a new post, assuming you have `hugo` installed...

#### If you don't have hugo installed...
See Hugo's quickstart guide [here](https://gohugo.io/getting-started/quick-start/).

*Ignore step 2 and step 3, we've already created the blog and the theme.*

#### Moving on...
At the *beginning* of every post, there is a little 'config' that'll allow you to set the title, date, author, description and cover image of the post.

There are **TWO** ways of setting up this config. They're very simple, and it doesn't matter which way you set up the config, as long as it's consistent in the current post. I.e. exactly one way described for one post, but another way can be used for another post.

##### First Way

```markdown
+++
title = ""
date = "2020-12-30"
author = ""
cover = "test.jpg"
description = ""
```

##### Second Way

```markdown
---
title: ""
date: ""
author: ""
description: ""
```

The only differences between these two are the replacement of the `=` -> `:` and the `+++` -> `---` respectively.

### Header Level 3

The header up above is written exactly as follows: `### Header Level 3`.

The code snippet below is exactly as follows: backticks are used to indicate code snippets.

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
Below, you'll find that bullet points and even dash-points work in levels of indentation. Pretty neat, right?

- Item 1
- Item 2
- Item 3
- Item 4
    - Item 4a
    - Item 4b
* Here, I'm using asterisks, but it comes out the same no matter what.
* Same here
    * Same here
1. Numbered item 1
2. Numbered item 2
3. Numbered item 3
4. Numbered item 4
    - Hmm, seems like you can't use dashes or asterisks with an indent underneath a numbered item

Aliquam erat volutpat. In hac habitasse platea dictumst. Nunc ut tincidunt mauris. Sed at gravida risus, id semper magna. Nullam vitae enim mattis, sodales neque non, pharetra elit. Cras sit amet sagittis augue, et finibus turpis. Ut tempus tincidunt diam vel pharetra. Nulla porttitor odio sit amet nulla scelerisque, quis aliquam mi imperdiet. Sed tincidunt dui vel tellus vestibulum rhoncus. Donec tempus ultrices velit.

