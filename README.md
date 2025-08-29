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
* Instructions for the grid that is used to layout the entire page. https://get.foundation/sites/docs-v5/

<details>
<summary>Unsure if these are actually useful </summary>
<ul>
 <li> https://getbootstrap.com/docs/4.2/layout/grid/ - unsure if we actually use bootstrap, and if this is the version we use.

</details>

### How the layouts work
#### Index
The index uses the `frontpage.html` layout, and also includes a masthead from `_masthead.html` if you use a `header` section in the frontmatter.

If you add a `white_space=true` to the frontmatter, it will add a small gap between the navigation bar and the masthead.

### Important Commands

* Run Locally: ``bundle exec jekyll serve --config _config.yml,_config_dev.yml``
* 

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
