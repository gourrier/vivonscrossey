# New README from Tatiana

## New Features
Phlow did a fantastic job with this template! I made the following upgrades and changes to suit my needs:

### Two Column Masthead with Image
`_includes/_masthead.html`, I added a new masthead type - two-column, which gives you an image on the left, and a title and text on the right.

To use this masthead, use the following in your frontmatter:
```
header: 
   white_space: true
   image_left: image-for-left-column.jpg
   title: Text for Header
   text: Text for your right column.  This will go into a div. <br> Use the break tag as before this paragraph for a new line, or: <p>surround each paragraph in paragraph tags.</p> You can use html tags like <a href="https://duckduckgo.com">links</a> in this section, but markdown won't work.
```

## Notes for Personal Use

### Important Internal Pages
* `_sass/_07_layout_scss` - explains the `class="t## b## r## l##"` stuff.
### Important Documentation Links:
* [Instructions for the grid that is used to layout the entire page from Foundation v5](https://get.foundation/sites/docs-v5/components/grid)
* [Kramdown Quick Reference](https://kramdown.gettalong.org/quickref.html)
* [feeling-responsive Template source code for documentation pages on Github](https://github.com/Phlow/feeling-responsive/tree/gh-pages/_posts/design)
  * The [Templates pages](https://phlow.github.io/feeling-responsive/design/) on the live feeling-responsive website.
  * The [Header examples](https://phlow.github.io/feeling-responsive/headers/) on the live feeling-responsive website
  * [General documentation](https://phlow.github.io/feeling-responsive/documentation/) on the live feeling-responsive website.

<details>
<summary>Unsure if these are actually useful </summary>
<ul>
 <li> https://getbootstrap.com/docs/4.2/layout/grid/ - unsure if we actually use bootstrap, and if this is the version we use.
</ul>
</details>

### My Dumb Questions
> And the Internet's answers.

<details>
<summary>What you'll find in this section</summary>
If I had to search my question online, and the solution was not immediately obvious in the first link in DuckDuckGo, I try to remember to write it down. This is where I'm writing it down for this website.  
This will include:  
* Tools, syntax, and features I should have known, but could not remember for the life of me.Hopefully writing it down helps cement it in my brain for next time.
* Things I've never had to do or implement, and had to had to look up.
* Bugs, glitches, and other issues that frustrated me.  
I do this to make these answers accessible in the future for both myself and anyone who (for some strange reason) refers to this project for information.  
Additionally, I want to explicitly acknowledge that I am learning as I work. I think that's one of my most valuable skills, and that it should be highlighted.  
And finally, I am a strong supporter of the open-source community, and a proponent of collaboration. I want to cite my sources, and highlight the people and websites that were most helpful to me.
</details>

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

### How the layouts work
#### Index
The index uses the `frontpage.html` layout, and also includes a masthead from `_masthead.html` if you use a `header` section in the frontmatter.

If you add a `white_space=true` to the frontmatter, it will add a small gap between the navigation bar and the masthead.

### Important Commands

* Run Locally: ``bundle exec jekyll serve --config _config.yml,_config_dev.yml``
* 


## TODOs:
- [ ] Make text wrap on two-column masthead
- [ ] Fix Github Pages Build Error: 
    * https://github.com/Phlow/feeling-responsive/issues/267
    * https://github.com/zerostaticthemes/jekyll-serif-theme/issues/91#issuecomment-2050033364
    * https://github.com/sieb/feeling-responsive/blob/gh-pages/.github/workflows/jekyll.yml

---
---
---
---

# Original README from Phlow

### You like and use this theme? Then support me. Just [paypal.me/PhlowMedia](https://www.paypal.me/PhlowMedia) :)

## Newsletter: Stay in Touch for Future Updates

If you are a webdesigner interested in Jekyll, the static website generator, this little newsletter is for you. I share tutorials, clever code snippets and information about my own Jekyll Themes called [*Feeling Responsive*][phlow7] and [*Simplicity*][phlow8]. Please don't expect weekly emails :)

[![Subscribe to Jekyll Newsletter](https://phlow.github.io/static/tinyletter_subscribe_button.png)](https://tinyletter.com/feeling-responsive)


[![Start Video](https://github.com/Phlow/feeling-responsive/blob/gh-pages/images/video-feeling-responsive-1280x720.jpg)](https://www.youtube.com/embed/3b5zCFSmVvU)

### A Responsive Jekyll Theme: *Feeling Responsive*

Do you want to get to know *Feeling Responsive*? Than check it out first and have a look on its home at  <http://phlow.github.io/feeling-responsive/>.

To get to know *Feeling Responsive* check out all the features explained in the [documentation][phlow1].

And what license is *Feeling Responsive* released under? [This one][phlow2].



### Why use this theme?

Feeling Responsive is heavily customizable.

1. Language-Support :)
2. Optimized for speed and it's responsive.
3. Built on Foundation Framework.
4. Six different Headers.
5. Customizable navigation, footer,...

**[More ›][phlow3]**



### Changelog

*Feeling Responsive* is in active development. Thank you to everyone who contributed, especially [Róbert Papp][phlow5], [Alexandra von Criegern](https://github.com/plutonik-a) and [Juan Jose Amor Iglesias](https://github.com/jjamor).

**[Read Changelog ›][phlow6]**



### Video Tutorial

Click the image to [watch the YouTube-Video-Tutorial][phlow4].

[![Start Video](https://github.com/Phlow/feeling-responsive/blob/gh-pages/images/video-feeling-responsive-tutorial-frontpage.jpg)](https://www.youtube.com/watch?v=rLS-BEvlEyY)








 [phlow1]: http://phlow.github.io/feeling-responsive/documentation/
 [phlow2]: https://github.com/Phlow/feeling-responsive/blob/gh-pages/LICENSE
 [phlow3]: http://phlow.github.io/feeling-responsive/info/
 [phlow4]: https://www.youtube.com/watch?v=rLS-BEvlEyY
 [phlow5]: https://github.com/TWiStErRob
 [phlow6]: https://phlow.github.io/feeling-responsive/changelog/
 [phlow7]: http://phlow.github.io/feeling-responsive/
 [phlow8]: http://phlow.github.io/simplicity/
 [phlow9]: #
 [phlow10]: #
