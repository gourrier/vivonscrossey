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
</ul>


#### Markdown


<ul class="accordion" data-accordion role="tablist">
    <li class="accordion-navigation">
        <a href="#MarkdownMultiParagraph" role="tab" id="MarkdownMultiParagraph-heading" aria-controls="MarkdownMultiParagraph">How do you do multi-paragraph footnotes? (or list items and similar)
            <div class="accordion-subtitle" markdown="1"> 
After the first paragraph, indent all other paragraphs by 4 spaces.
</div>
        </a>
        <div id="MarkdownMultiParagraph" class="content" role="tabpanel" aria-labelledby="MarkdownMultiParagraph-heading" markdown="1">

##### Sources: 
* <https://www.hardscrabble.net/2023/multi-paragraph-footnotes-in-markdown/>
##### Code Example:
 
```
Some text with a footnote.[^bignote]

---
[^bignote]: Here's one with multiple paragraphs and code.

    Indent paragraphs by 4 spaces to include them in the footnote.

    `{ my code }`

    Add as many paragraphs as you like
```

##### Result: 
Some text with a footnote.[^bignote]

---
[^bignote]: Here's one with multiple paragraphs and code.

    Indent paragraphs by 4 spaces to include them in the footnote.

    `{ my code }`

    Add as many paragraphs as you like


</div>
    </li>
    <li class="accordion-navigation">
        <a href="#MarkdownHTML" role="tab" id="MarkdownHTML-heading" aria-controls="MarkdownHTML">How do I include HTML/CSS in my Markdown document?
            <div class="accordion-subtitle" markdown="1"> 
HTML elements work natively in Markdown documents.
</div>
        </a>
        <div id="MarkdownHTML" class="content" role="tabpanel" aria-labelledby="MarkdownHTML-heading" markdown="1">

##### Sources 
* [Michael Currin's answer on the Jekyll Forums](https://talk.jekyllrb.com/t/html-in-markdown/4585/2)
* And the [original Markdown instruction manual section](https://daringfireball.net/projects/markdown/syntax#html) that he links to
##### Code Example:** 

```
I am writing a paragraph in Markdown.

<h2 style="border-style: solid;">This is a custom header </h2>

I used an HTML tag with CSS elements in the tag, and it should just work.

<h2 style="border-style: solid;">This **Header** has unparsed _markdown_ styling </h2>

This paragraph has markdown styling. **This would show up bold** and _this would show up italic_. I used the same markdown styling in the header - but the header would show the asterisks and underlines, not the styles they represent.
```

##### Result: 
I am writing a paragraph in Markdown.

<h2 style="border-style: solid;">This is a custom header </h2>

I used an HTML tag with CSS elements in the tag, and it should just work.

<h2 style="border-style: solid;">This **Header** has unparsed _markdown_ styling </h2>

This paragraph has markdown styling. **This would show up bold** and _this would show up italic_. I used the same markdown styling in the header - but the header would show the asterisks and underlines, not the styles they represent.

</div>
    </li>
    <li class="accordion-navigation">
        <a href="#MarkdownCSS" role="tab" id="MarkdownCSS-heading" aria-controls="MarkdownCSS">How do I use CSS classes and styles in my markdown styles?<p class="accordion-subtitle" markdown="1">
Kramdown allows block-level class, style, and ID definitions using `{: .class attribute="value" #givenID}` after the block
</p>
        </a>
        <div id="MarkdownCSS" class="content" role="tabpanel" aria-labelledby="MarkdownCSS-heading" markdown="1">

##### Sources
* https://kramdown.gettalong.org/quickref.html#block-attributes
##### Code Example:

```
## A Heading that I want to color and name 
{: style="color: red"} 

A paragraph that I want in a foundation panel.  These classes are introduced by Foundation, which this website uses, but are not universal to HTML/CSS.
{: .panel .radius}

A paragraph referring back to a [previous header](#ArbitraryIdentifier).
```

##### Result

## A Heading that I want to color and name
{: style="color: red;" #ArbitraryIdentifier}

A paragraph that I want in a foundation panel.  These classes are introduced by Foundation, which this website uses, but are not universal to HTML/CSS.
{: .panel .radius}

A paragraph referring back to a [previous header](#ArbitraryIdentifier).
</div>
    </li>
    <li class="accordion-navigation">
        <a href="#KramdownHTML" role="tab" id="KramdownHTML-heading" aria-controls="KramdownHTML">How do I use Markdown in my HTML elements/documents?<div class="accordion-subtitle" markdown="1">
Kramdown allows markdown parsing within (most) spans and blocks using the `markdown=` attribute
</div>
        </a>
        <div id="KramdownHTML" class="content" role="tabpanel" aria-labelledby="KramdownHTML-heading" markdown="1">

##### Discussion
I knew this one was possible, but I kept running into issues, and finding my source for this knowledge was incredibly difficult while I was trying to troubleshoot.  So I've included several explanations and examples in the sources.

This has worked fairly consistently for me, using `markdown="span"` or `markdown="block"` in the html tags as needed.  **However**, within the YAML headers, this doesn't seem to work.

The content in the YAML headers that gets inserted into the page parses as Markdown/Kramdown, and the HTML tags in that content get used as HTML like they would in a .md document.  But including the `markdown` attribute in the HTML tag does not allow markdown within the HTML span or block in the YAML header to be parsed as markdown.

I hypothesize that this is because the YAML headers are parsed by Liquid, and that the Liquid markdown parser is using a flavor of markdown that does not support the `markdown` attribute, rather than the Kramdown parser that Jekyll is using from my `_config.yaml` settings.

The `markdown` attribute also breaks accordion titles with subtitles, in the way that I've implemented them.
##### Sources
* <https://stackoverflow.com/questions/22291211/jekyll-how-to-get-markdown-parsing-inside-blocks-using-kramdown>
* <https://kramdown.gettalong.org/syntax.html#html-blocks>
* <https://kramdown.gettalong.org/syntax.html#html-spans>
* <https://kylebebak.github.io/post/mixing-markdown-html>

##### Example
```
[code stuff TBD]
```

##### Result
TBD
</div>
    </li>
</ul>
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
