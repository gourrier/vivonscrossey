---
layout: page-fullwidth
title: "Website Element Blocks"
subheadline: "For the forgetful blogger"
teaser: "The building blocks of this website"
permalink: "/readme/elements"
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

## Basic Markdown

There are a ton of websites that talk about basic markdown.  The Kramdown website is a good resource.

## Foundation Elements

### Vanilla Foundation

Foundation defines a lot of building blocks we can use.  These are the ones that are identical to how Foundation says to use it, and how they say to use it.

### Customized Foundation Elements

I've defined custom CSS and features for some of the built-in Foundation elements.  These are the ones that I've customized, or that have quirks related to my standard use, that Foundation doesn't cover in their documentation.

#### Accordions

<ul class="accordion" data-accordion role="tablist">
    <li class="accordion-navigation">
        <a href="#panelIDNumberOrName" role="tab" id="panelIDNumberOrName-heading" aria-controls="panelIDNumberOrName">The title of your accordion - or question if it's an FAQ
            <div class="accordion-subtitle" markdown="1"> 
The subtitle of your accordion, italicized and indented.  **Markdown** works in this section, and it's a good spot for a short FAQ answer
</div>
        </a>
        <div id="panelIDNumberOrName" class="content" role="tabpanel" aria-labelledby="panelIDNumberOrName-heading" markdown="1">
The content inside the accordion.  This can use **markdown** like:

* Bullet points
* [Links](/readme)
##### Headings

Multiple paragraphs. Like this.

{% highlight html %}
<p>Code Blocks</p>
{% endhighlight %}

The important thing to remember is that the markdown needs to stay ALL THE WAY unindented, even if the section it's in is indented.  And the HTML closing tag needs to be on a newline and unindented, if the markdown is being processed as a block (compared to as a span).


</div>
    </li>
    <li class="accordion-navigation">
        <a href="#anotherpanelIDNumberOrName" role="tab" id="anotherpanelIDNumberOrName-heading" aria-controls="anotherpanelIDNumberOrName">The HTML for an accordion <div class="accordion-subtitle"> In fact, the HTML for THIS accordion </div> </a>
        <div id="anotherpanelIDNumberOrName" class="content" role="tabpanel" aria-labelledby="anotherpanelIDNumberOrName-heading" markdown="1">
The content inside the accordion.  This can use **markdown** like:

{% highlight html %}
<ul class="accordion" data-accordion role="tablist">
    <li class="accordion-navigation">
        <a href="#panelIDNumberOrName" role="tab" id="panelIDNumberOrName-heading" aria-controls="panelIDNumberOrName">The title of your accordion - or question if it's an FAQ
            <div class="accordion-subtitle" markdown="1"> 
The subtitle of your accordion, italicized and indented.  **Markdown** works in this section, and it's a good spot for a short FAQ answer
</div>
        </a>
        <div id="panelIDNumberOrName" class="content" role="tabpanel" aria-labelledby="panelIDNumberOrName-heading" markdown="1">
The content inside the accordion.  This can use **markdown** like:

* Bullet points
* [Links](/readme)
##### Headings

Multiple paragraphs. Like this.

{% raw %}
{% highlight html %}
<p>Code Blocks</p>
{% endhighlight %}
{% endraw %}

The important thing to remember is that the markdown needs to stay ALL THE WAY unindented, even if the section it's in is indented.  And the HTML closing tag needs to be on a newline and unindented, if the markdown is being processed as a block (compared to as a span).


</div>
    </li>
    <li class="accordion-navigation">
        <a href="#anotherpanelIDNumberOrName" role="tab" id="anotherpanelIDNumberOrName-heading" aria-controls="anotherpanelIDNumberOrName">The HTML for an accordion <div class="accordion-subtitle"> In fact, the HTML for THIS accordion </div> </a>
        <div id="anotherpanelIDNumberOrName" class="content" role="tabpanel" aria-labelledby="anotherpanelIDNumberOrName-heading" markdown="1">
The content inside the accordion.  This can use **markdown** like:

{% raw %}
{% highlight html %}
[excluded due to recursion]
{% endhighlight %}
{% endraw %}


</div>
    </li>
</ul>
{% endhighlight %}


</div>
    </li>
</ul>
