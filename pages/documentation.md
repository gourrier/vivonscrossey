---
layout: page-fullwidth
title: "Website Creation Documentation"
subheadline: "A better README"
teaser: "The documentation is a work in progress..."
permalink: "/readme/"
header:
   image_fullwidth: "header_roadmap_2.jpg"
---
<div class="row">
<div class="medium-4 medium-push-8 columns" markdown="1">
<div class="panel radius" markdown="1">
**Table of Contents**
{: #toc }
*  TOC
{:toc}
</div>
</div><!-- /.medium-4.columns -->

<div class="medium-8 medium-pull-4 columns" markdown="1">

## Notes for Personal Use

### Important Internal Pages

* `_sass/_07_layout_scss` - explains the `class="t## b## r## l##"` stuff.

### Important Documentation Links:

* Foundation Info
  * [The Kitchen Sink](https://get.foundation/sites/docs-v5/components/kitchen_sink.html#build)
  * [Instructions for the grid that is used to layout the entire page from Foundation v5](https://get.foundation/sites/docs-v5/components/grid)
  * [Utility classes introduced by Foundation](https://get.foundation/sites/docs-v5/utility-classes.html) such as alignment and location, and radiusing boxes.
  * [Accordions](https://get.foundation/sites/docs-v5/components/accordion.html)
* [Kramdown Quick Reference](https://kramdown.gettalong.org/quickref.html)
* [feeling-responsive Template source code for documentation pages on Github](https://github.com/Phlow/feeling-responsive/tree/gh-pages/_posts/design)
  * The [Templates pages](https://phlow.github.io/feeling-responsive/design/) on the live feeling-responsive website.
  * The [Header examples](https://phlow.github.io/feeling-responsive/headers/) on the live feeling-responsive website
  * [General documentation](https://phlow.github.io/feeling-responsive/documentation/) on the live feeling-responsive website.

I'm unsure if these are actually useful, but: 
<ul>
 <li> https://getbootstrap.com/docs/4.2/layout/grid/ - unsure if we actually use bootstrap, and if this is the version we use.</li>
 <li> A custom jekyll plugin for liquid accordions, that I can't use because I'm hosting this site on Github. https://mikelui.io/2018/07/22/jekyll-nested-blocks.html </li>
</ul>

### Stuff Other People Made

* The script for autoscrolling when opening accordions that I added to `_footer_scripts` is a near copy-paste from [Bricklabs' page on this topic.](https://brickslabs.com/automatically-scroll-to-the-open-accordion-item/).  I had to change the `const accordionHeader` to `.accordion-navigation` to match Foundation's syntax, but that was it - it just works.

### My Dumb Questions
> And the Internet's answers.

<ul class="accordion" data-accordion data-multi-expand="true" role="tablist">
    <li class="accordion-navigation">
        <a href="#panel1" role="tab" id="panel1-heading" aria-controls="panel1">What you'll find in this section
            <div class="accordion-subtitle"> A lot, it turns out.
            </div>
        </a>
        <div id="panel1" class="content" role="tabpanel" aria-labelledby="panel1-heading" markdown="1">
If I had to search my question online, and the solution was not immediately obvious in the first link in DuckDuckGo, I try to remember to write it down. This is where I'm writing it down for this website.  

This will include:  
* Tools, syntax, and features I should have known, but could not remember for the life of me. Hopefully writing it down helps cement it in my brain for next time.
* Things I've never had to do or implement, and had to had to look up.
* Bugs, glitches, and other issues that frustrated me.

I do this to make these answers accessible in the future for both myself and anyone who (for some strange reason) refers to this project for information.  

Additionally, I want to explicitly acknowledge that I am learning as I work. I think that's one of my most valuable skills, and that it should be highlighted.  

And finally, I am a strong supporter of the open-source community, and a proponent of collaboration. I want to cite my sources, and highlight the people and websites that were most helpful to me.
</div>
    </li>
    <li class="accordion-navigation">
        <a href="#panel2d"  role="tab" id="panel2d-heading" aria-controls="panel2d">What you'll find in this section <div class="accordion-subtitle"> A lot, it turns out.</div></a>
        <div id="panel2d" class="content" role="tabpanel" aria-labelledby="panel2d-heading">
If I had to search my question online, and the solution was not immediately obvious in the first link in DuckDuckGo, I try to remember to write it down. This is where I'm writing it down for this website.  

This will include:  
* Tools, syntax, and features I should have known, but could not remember for the life of me. Hopefully writing it down helps cement it in my brain for next time.
* Things I've never had to do or implement, and had to had to look up.
* Bugs, glitches, and other issues that frustrated me.

I do this to make these answers accessible in the future for both myself and anyone who (for some strange reason) refers to this project for information.  

Additionally, I want to explicitly acknowledge that I am learning as I work. I think that's one of my most valuable skills, and that it should be highlighted.  

And finally, I am a strong supporter of the open-source community, and a proponent of collaboration. I want to cite my sources, and highlight the people and websites that were most helpful to me.
</div>
    </li>
    <li class="accordion-navigation">
        <a href="#panel2X"  role="tab" id="panel2d-heading" aria-controls="panel2X">What you'll find in this section 2X <div class="accordion-subtitle"> A lot, it turns out.</div></a>
        <div id="panel2X" class="content" role="tabpanel" aria-labelledby="panel2X-heading">
If I had to search my question online, and the solution was not immediately obvious in the first link in DuckDuckGo, I try to remember to write it down. This is where I'm writing it down for this website.  

This will include:  
* Tools, syntax, and features I should have known, but could not remember for the life of me. Hopefully writing it down helps cement it in my brain for next time.
* Things I've never had to do or implement, and had to had to look up.
* Bugs, glitches, and other issues that frustrated me.

I do this to make these answers accessible in the future for both myself and anyone who (for some strange reason) refers to this project for information.  

Additionally, I want to explicitly acknowledge that I am learning as I work. I think that's one of my most valuable skills, and that it should be highlighted.  

And finally, I am a strong supporter of the open-source community, and a proponent of collaboration. I want to cite my sources, and highlight the people and websites that were most helpful to me.
</div>
    </li>
    <li class="accordion-navigation">
        <a href="#panel3d" role="tab" id="panel3d-heading" aria-controls="panel3d">Accordion 3</a>
        <div id="panel3d" class="content" role="tabpanel" aria-labelledby="panel3d-heading">
      Panel 3. Lorem ipsum dolor
        </div>
    </li>
</ul>


<dl class="accordion" data-accordion role="tablist">
    <dd class="accordion-navigation">
        <a href="#paneltest2"  role="tab" id="paneltest2-heading" aria-controls="paneltest2">Accordion 2</a>
        <div id="paneltest2" class="content" role="tabpanel" aria-labelledby="paneltest2-heading">
      Panel 2. Lorem ipsum dolor
        </div>
    </dd>
    <dd class="accordion-navigation">
        <a href="#paneltest3" role="tab" id="paneltest3-heading" aria-controls="paneltest3">Accordion 3</a>
        <div id="paneltest3" class="content" role="tabpanel" aria-labelledby="paneltest3-heading">
      Panel 3. Lorem ipsum dolor
        </div>
    </dd>
</dl>


#### Markdown

* **How do you do multi-paragraph footnotes? (or lists and similar.)**
  * After the first paragraph, indent all other paragraphs by 4 spaces
    * Source: <https://www.hardscrabble.net/2023/multi-paragraph-footnotes-in-markdown/>
    * Example:
 
        ```
        Some text.[^bignote]

        ---
        [^bignote]: Here's one with multiple paragraphs and code.

            Indent paragraphs by 4 spaces to include them in the footnote.

            `{ my code }`

            Add as many paragraphs as you like
        ```

* **How do I include HTML/CSS in my Markdown document, and use Markdown in my HTML elements/documents?**
    <details><summary>HTML elements work natively in Markdown documents.</summary>
    **Source:** 
    * [Michael Currin's answer on the Jekyll Forums](https://talk.jekyllrb.com/t/html-in-markdown/4585/2)
    * And the [original Markdown instruction manual section](https://daringfireball.net/projects/markdown/syntax#html) that he links to
    **Example:** 

    ```
    I am writing a paragraph in Markdown.

    <h2 style="border-style: solid;">This is a custom header </h2>

    I used an HTML tag with CSS elements in the tag, and it should just work.

    <h2 style="border-style: solid;">This **Header** has unparsed _markdown_ styling </h2>

    This paragraph has markdown styling. **This would show up bold** and _this would show up italic_. I used the same markdown styling in the hdeader - but the header would show the asterisks and underlines, not the styles they represent.
    ```
    </details>
    <details><summary>Kramdown allows block-level class, style, and ID definitions using `{: .class attribute="value" #givenID} after the block</summary>
    **Source:** https://kramdown.gettalong.org/quickref.html#block-attributes
    **Example:** 
    ```
    ## A Heading that I want to outline and name
    {: border-style="solid" #ArbitraryIdentifier}

    A paragraph that I want in a foundation panel.  These classes are introduced by Foundation, which this website uses, but are not universal to HTML/CSS.
    {: .panel .radius}
    ```
    </details>
    <details><summary>Kramdown allows markdown parsing within (most) spans and blocks using the `markdown=` attribute</summary>
    I knew this one was possible, but I kept running into issues, and finding my source for this knowledge was incredibly difficult while I was trying to troubleshoot.  So I've included several explanations and examples in the sources.
    This has worked fairly consistently for me, using `markdown="span"` or `markdown="block"` in the html tags as needed.  **However**, within the YAML headers, this doesn't seem to work.
    The content in the YAML headers that gets inserted into the page parses as Markdown/Kramdown, and the HTML tags in that content get used as HTML like they would in a .md document.  But including the `markdown` attribute in the HTML tag does not allow markdown within the HTML span or block in the YAML header to be parsed as markdown.
    I hypothesize that this is because the YAML headers are parsed by Liquid, and that the Liquid markdown parser is using a flavor of markdown that does not support the `markdown` attribute, rather than the Kramdown parser that Jekyll is using from my `_config.yaml` settings.
    The `markdown` attribute also breaks accordion titles with subtitles, in the way that I've implemented them.
    **Source:**
    * https://stackoverflow.com/questions/22291211/jekyll-how-to-get-markdown-parsing-inside-blocks-using-kramdown
    * https://kramdown.gettalong.org/syntax.html#html-blocks
    * https://kramdown.gettalong.org/syntax.html#html-spans
    * https://kylebebak.github.io/post/mixing-markdown-html
    **Example:**
    ```
    [code stuff]
    ```
    </details>
* **[Question?]**
    <details><summary>[Short answer]</summary>
    [Longer description/Explanation]
    **Source:** [Single Source Link]
    * [If more than one source link]
    * [Put them all in a list]
    **Example:** 

    ```
    [Example of how to do the thing]
    ```
    </details>

#### CSS

* **How do I make my photo circular?**
    <details><summary>[Short answer]</summary>
    [Longer description/Explanation]
    **Source:** [Single Source Link]
    * [If more than one source link]
    * [Put them all in a list]
    **Example:** 

    ```
    [Example of how to do the thing]
    ```
    </details>

* **What's the difference between `.` and `#` in the CSS style selectors?**
    <details><summary> `.` refers to a class - a set of attributes shared by multiple items.  `#` refers to an ID - a tag that only one item on a page can have.</summary>
    **Source:** <https://stackoverflow.com/questions/602168/in-css-what-is-the-difference-between-and-when-declaring-a-set-of-styles>
    </details>

#### Foundation

**Why is the accordion being dumb?**

Lots of reasons, honey. Lots of reasons.  But this is the one you were working on when you asked this question.  https://stackoverflow.com/questions/41576713/custom-arrow-up-down-accordion-vertical-menu-foundation-6

You're using an earlier version of foundation, so the syntax is different, but you can see what you did in _custom.scss.

#### Misc.

* **Why am I getting some random latin characters on my 404 page when I host my site locally?**
    <details><summary> This happens when the text is encoded with the Windows-1252 character encoding, and decoded with the ISO-8859-1 character encoding of the characters.  </summary>
    This was a weird bug to figure out.  On my live website, built and hosted by Github, everything looked fine.  When I hosted the site locally, using `bundle exec jekyll serve` and went to `localhost:4000/404`, it looked fine.

    However, if hosted the site locally, and went to a page that *redirected* to the 404 page, some characters like `...` and &rarr; would get encoded as 3 seemingly arbitrary latin characters or diacritics.

    I went through a few steps to troubleshoot this.
    * First, the [UTF-8 Encoding Debug Table](https://www.i18nqa.com/debug/utf8-debug.html) made it clear that that my special characters were being encoded using the Windows-1252 character encoding, but being treated as plain UTF-8 or ISO-8559 encoded characters when they were being displayed.
    * My code was right - all the configs were set for UTF-8 character encoding (except in SVGs that I wasn't worried about anyway)
    * My IDE, Visual Studio Code, was also claiming to be using UTF-8 for encoding and decoding files.
    * For a minute I thought that the issue was the template itself
      * The template was made by an apparent German-speaker
      * Some of the common symbols used suggested they used a non-English keyboard - in fact, I first noticed this issue as I was replacing the `&gt;` symbols in some of the files.
      * However, changing the symbols to english-keyboard equivalents didn't fix the problem, and neither did resaving the markdown files with VSCode (which, again, was claiming to use UTF-8 encoding).
    * Because this was only happening on local hosting, it suggested that this was a problem with my computer itself, not with the markdown.
      * I was able to identify that, despite VSCode using UTF-8, the PowerShell terminal inside VSCode was using Windows-1252 character encoding with the `[System.Text.Encoding]::Default` command.
    * I checked `chcp.com` in my command line to check that status, but didn't want to mess with my computer too much.
    * Since the issue was unique to redirects, I went into the `redirect.html` file to see if I could fix it there by moving the charset declaration to the top of the `&lt;head&gt;` declaration.  It didn't seem to work.
    * At this point, I did something smart - I tested my website on a different browser.  
      * Shockingly, the page was fine on both Microsoft Edge and Google Chrome.  And then, it was also fine on a fresh Firefox profile.  But it was still wrong on my standard Firefox profile.
    * And finally, I cleared the cache on my Firefox profile.  I deleted all data related to `localhost:4000`, and reloaded the page.
    And. . . it worked.  The errant characters rendered properly.
    It took me far too long to fix this issue.  I probably *shouldn't have* bothered to fix it, since it did not actually affect the live site and I had actual content to work on.
    But it did teach me about character encoding and meta tags, and prompted me to set up a quick cache-clear button on my firefox profile.

    **Source:**
    * [UTF-8 Encoding Debug Table](https://www.i18nqa.com/debug/utf8-debug.html)
    * Person who talked about the charset page thing and how to tell what section my computer was set to.
    * [A page about Windows-1252](https://mojoauth.com/compare-character-encoding/windows-1252-vs-windows-1255/)
    * A StackOverflow conversation about [A Jekyll bug regarding character encoding](https://stackoverflow.com/questions/13146420/my-jekyll-site-cant-build-liquid-exception-incompatible-character-encodings)
    * A github issue report about [UTF-8 files outputting with incompatible character encodings](https://github.com/jekyll/jekyll/issues/5584)
    * An official page with [instructions on declaring encoding as UTF-8](https://www.w3.org/International/questions/qa-changing-encoding.en)




## Edit Navigation   {#edit-navigation}

To customize the navigation of *Feeling Responsive*, edit the [YAML](https://jekyllrb.com/docs/datafiles/)-file `_data/navigation.yml`.

## Different Page/Posts Formats   {#formats}

*Feeling Responsive* supports you with different templates for your content. These are the actual page/post formats:

### Page/Post
The [page/post format]({{ site.url }}{{ site.baseurl }}/design/page/) has no sidebar by default, its content is centered and beneath the content the visitor gets some metadata like categories, tags, date and author if provided via data in front matter of the post.

use in front matter via: `layout: page`

### Page/Post with a left or right sidebar
If you want to show the sidebar, just enter `sidebar: left` or `sidebar: right` in front matter, and *whoops, there it is*! To customize the content of the sidebar, open `_includes/sidebar`.


### Page/Post with or without metadata
You can show metadata, such as categories, tags and a date at the end of the page, just enter `show_meta: true`. By default, it's turned on. You can change it via `_config.yml`. To turn off metadata, enter `show_meta: false`.



### Page Full Width
If you want full control of styling a page, then use the [page fullwidth template]({{ site.url }}{{ site.baseurl }}/design/page-fullwidth/). To set up a grid, just use the [foundation grid system](http://foundation.zurb.com/docs/components/grid.html).

use in front matter via: `layout: page-fullwidth`


### Frontpage
This template is special. It allows you to define three *widgets* which are displayed with a headline, image, description and a link to the content. It's used for the [homepage]({{ site.url }}{{ site.baseurl }}) of this website.

use in front matter via: `layout: frontpage`


### Video
If you're a video producer or cineast, you'll like the [video template]({{ site.url }}{{ site.baseurl }}/design/video/). It darkens the layout to black and lets the video stand out full-width.

use in front matter via: `layout: video`

<small markdown="1">[Up to table of contents](#toc)</small>
{: .text-right }

## Style your content with   {#styling}

Feeling Responsive offers different options to style your article content. There are elements like subheadlines, feature images, header images, homepage images, meta data like categories and tags and many more.


### subheadlines

If you need a subheadline for an article, just define a subheadline in front matter like this:

`subheadline:  "Subheadline"`

### Quotes

Quotes mix it up a little bit, if you write long articles. So use quotes:

> Age is an issue of mind over matter. If you don't mind, it doesn't matter.
<cite>Mark Twain</cite>

<small markdown="1">[Up to table of contents](#toc)</small>
{: .text-right }

{% highlight html %}
> Age is an issue of mind over matter. If you don't mind, it doesn't matter.
<cite>Mark Twain</cite>
<small markdown="1">[Up to table of contents](#toc)</small>
{: .text-right }
{% endhighlight %}

## Comments

You can use comments with *Feeling Responsive* by the way of Disqus. If you want to use Disqus-Comments just open `config.yml` and add your `disqus_shortname`. [More on how to use Disqus ›](https://disqus.com/websites/)

By default comments are turned off. You can customize the default behaviour in `config.yml`. To **turn on comments** just add `comments: true` to front matter using the page layout `layout: page`. 

<small markdown="1">[Up to table of contents](#toc)</small>
{: .text-right }

## Responsive Videos

With foundation, responsive videos are easy. [More ›](http://foundation.zurb.com/docs/components/flex_video.html)

<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/WoHxoz_0ykI" frameborder="0" allowfullscreen></iframe>
</div>

### Code to use for flexible videos

{% highlight html %}
<div class="flex-video">
  <iframe with video />
</div>
{% endhighlight %}


<img class="t60" src="{{ site.urlimg }}header_homepage_13.jpg" alt="">

## Images: Title, Thumbnails, Homepage   {#images}

There are several types of images you can define via front matter. If you want to change the images used in the header, have a look at [Style your Header]({{ site.url }}{{ site.baseurl }}/headers/). 


### Title Images

~~~
image:
    title: image.jpg
~~~


### Thumbnails

Thumbnails are used on archive pages like the [blog index][2]. They have a size of 150x150 pixels. Define them in front matter like this:

~~~
image:
    thumb: thumbnail_image.jpg
~~~


### Homepage Image

If you want to feature an article on the homepage with a huge image, then use the homepage image with a width of 970 pixels. If no homepage image is defined *Feeling Responsive* writes instead *New Blog Articles* over the blog entries. Define the homepage image like this:

~~~
image:
    homepage: header_homepage_13.jpg
~~~

### Captions with URL

Sometimes, you want to give credit to the creator of your images, maybe with a link. Especially when you use Creative Commons-images like I do for this website. Just add the following front matter and *Feeling Responsive* does the rest:

~~~
image:
    title: header_image.jpg
    caption: Image by Phlow
    caption_url: "http://phlow.de/"
~~~

### Define all images for an article

~~~
image:
    title: title_image.jpg
    thumb: thumbnail_image.jpg
    homepage: header_homepage_13.jpg
    caption: Image by Phlow
    caption_url: "http://phlow.de/"
~~~


<small markdown="1">[Up to table of contents](#toc)</small>
{: .text-right }


## Create a Table of Contents
{: .t60}

With the Kramdown parser for Markdown, you can render a table of contents for your documents. Just insert the following HTML in your post before the actual content. More information on [»Automatic ›Table of Contents‹ Generation«][1].

### Bare Bones Version
{% highlight html %}
### Table of Contents
*  Auto generated table of contents
{:toc}
{% endhighlight %}

### Foundation panel version

{% highlight html %}
<div class="panel radius" markdown="1">
**Table of Contents**
{: #toc }
*  TOC
{:toc}
</div>
{% endhighlight %}
<small markdown="1">[Up to table of contents](#toc)</small>
{: .text-right }

## Breadcrumbs

To turn on breadcrumbs, just use...

{% highlight html %}
breadcrumb: true
{% endhighlight %}


## Includes
{: .t60}

Includes can be very helpful to spice up your content. You can use includes in your Markdown-files with ease: Just call them with some Liquid code.

### list-posts.html

The `list-posts.html`-include is a loop to list posts. It's a helper to add some additional content fast and easy. You can use it in individual posts for example. Which parameters you use, depends on you.

Possible parameter for the loop:

- entries › define the number of entries to show
- offset › define the offset (number of entries to skip before displaying the first one)
- category › define **only one** category to display according entries

The loop looks like this when you use all parameters. Single parameters are possible of course.

~~~
{% raw %}{% include list-posts entries='3' offset='1' category='design' %}{% endraw %}
~~~

### next-previous-post-in-category.html

This include creates a next/previous link to a post of the same category using the first categories-variable in front matter.

~~~
{% raw %} {% include next-previous-post-in-category %}{% endraw %}
~~~

### improve_content

If your content is on Jekyll, you can use this include to automatically generate a »Edit on GitHub Link« to give people a possibility to improve your content. Got the idea from [Ben Balters Blog](http://ben.balter.com/).

~~~
{% raw %}{% include _improve_content.html %}{% endraw %}
~~~

### list-collection

This include lets you loop through a collection to list all entries in that collection. If you set »published: false« in front matter of a collection page, the page gots filtered out via unless. The following example loops through a collection called *wordpress*.

~~~
{% raw %}{% include list-collection collection='wordpress' %}{% endraw %}
~~~

### alert – Embed an alert in your content

This include lets you easily display an alert. To use the include, no `.html` ending is necessary. You can use five different kinds of alerts: `warning`, `info`, `success`, `alert` and `text`. 

~~~
{% raw %}{% include alert warning='This is a warning.' %}
{% include alert info='An info box.' %}
{% include alert success='Yeah, you made it!' %}
{% include alert alert='Danger!' %}
{% include alert terminal='jekyll -serve' %}
{% include alert text='Just a note!' %}{% endraw %}
~~~

{% include alert warning='This is a warning.' %}
{% include alert info='An info box.' %}
{% include alert success='Yeah, you made it!' %}
{% include alert alert='Danger!' %}
{% include alert terminal='jekyll -serve' %}
{% include alert text='Just a note!' %}

You can even use `<html>`-tags inside the alert. Beware: Use " and ' properly.

~~~
{% raw %}{% include alert info='<em>Feeling Responsive</em> is listed on <a href="http://jekyllthemes.org/">http://jekyllthemes.org</a>' %}{% endraw %}
~~~

{% include alert info='<em>Feeling Responsive</em> is listed on <a href="http://jekyllthemes.org/">http://jekyllthemes.org</a>' %}

<small markdown="1">[Up to table of contents](#toc)</small>
{: .text-right }

## Javascript/Foundation modules

*Feeling Responsive* uses the foundation framework and some of its Javascript components. I reduced the modules, to decrease page load and make the theme faster.

I only added one other javascript-module: [`backstretch`][3] by Scott Robbin. These modules are currently used by the theme and included in `javascript.min.js`. There is also a non-minified version, if you want to take a closer look: `javascript.js`.

~~~
/foundation/bower_components/foundation/js/vendor/jquery.js'
/foundation/bower_components/foundation/js/vendor/fastclick.js'
/foundation/bower_components/foundation/js/foundation.accordion.js'
/foundation/bower_components/foundation/js/foundation.clearing.js'
/foundation/bower_components/foundation/js/foundation.dropdown.js'
/foundation/bower_components/foundation/js/foundation.equalizer.js'
/foundation/bower_components/foundation/js/foundation.magellan.js'
/foundation/bower_components/foundation/js/foundation.topbar.js'
/foundation/js/jquery.backstretch.js'
~~~

{% include _improve_content.html %}

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->

 [1]: http://kramdown.gettalong.org/converter/html.html#toc
 [2]: {{ site.url }}/blog/
 [3]: http://srobbin.com/jquery-plugins/backstretch/
 [4]: #
 [5]: #
 [6]: #
 [7]: #
 [8]: #
 [9]: #
 [10]: #
