# bisl-theme
A little theme for the [Hugo blogging framework](https://gohugo.io/), developed for my site tech.taymor.io. It presumes you [celebrate acheivements with donuts](http://larahogan.me/donuts/). It is designed to host a basic portfolio site and blog.

What is a bisl? In Yiddish, [a bisl](http://www.jewish-languages.org/jewish-english-lexicon/words/67) is a little bit. Bisl-theme is a stylistically little Hugo theme, with minimalist design. We don't, however, have a bisl of opinions that you should celebrate your career acheivements with donuts. We have a lot.

## To Install

```
$ cd <hugo repo root dir>
$ git submodule add https://github.com/ctaymor/bisl-theme.git themes/bisl
$ git submodule init
$ git submodule update
```

## Archetypes:
### Posts:

The frontmatter for your posts should include:
key | used for 
----|------------------------
title | The name of the blogpost. This will be used for the link, the top of the post, and also as the title for the webpage in the metadata, so best to keep it short and simple
date | The date you want the page to display as posted 
tags | any categories related to your blogpost. Currently unused
draft | false if post is ready for publication
showDate | true or false. If true, the blogpost date will be displayed. If not, the blogpost date will not be displayed anywhere. Use false for always relevant posts.

You can add an index page at `content/posts/_index.html` with an introduction and title for your list of blogposts if you wish.

### Donuts:

The frontmatter for your donuts should include:
key      | used for
--------|----------------------
title | not currently used
description | what did you acheive to earn a donut? Remember, donuts are cheap. It doesn't have to be a BIG accomplishment to celebrate. Celebrate even your little acheivements.
alt_text | A description of your image. Very important for accessibility for people who use screen readers. Don't leave this out. Keep it short and sweet. For instance: "a person holding a blueberry donut"
image_src | A link to your image hosted on the web. It should be 375x375 pixels. I use google cloud storage
donut_type | what delicious flavor of donut did you enjoy?
date | When did you do the accomplishement?
draft | false to publish. (But maybe it's a secret project you can't share yet, in which case set it true)

You might wish to include an _index.html file in `content/donuts`. This will display above the list of donuts.
May we suggest something like this:

```
Inspired by <a href="http://larahogan.me/donuts/">Lara Hogan</a>, <a href="https://beero.ps/cupcakes/">Ryn Daniels</a> and <a href="https://tech.taymor.io/donuts">Caroline Taymor</a>, I'm celebrating my acheivements with donuts. It's easy not to notice the little accomplishments in our lives and work, and not notice our growth. By taking the time to enjoy a tasty treat and reflect on my accomplishment, and documenting doing so, I'm practicing noticing my growth and accomplishments.
```
