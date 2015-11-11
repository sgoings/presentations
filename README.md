# presentations

Collection of presentations given by the Deis team using:

- [Markdown][] for less markup
- [Reveal.js][] for presentations
- [Jekyll][] for site management

## Getting Started

1. [install Jekyll][]. After that, clone this repository:

        git clone --recursive https://github.com/sgoings/presentations.git

2. add your presentation into the *_posts* subdirectory with the common Jekyll
naming scheme
3. start writing in Markdown. You can preview your post via:

        make serve

## Configuring the presentations

You can configure almost any reveal.js setting using the _config.yml-settings file in the
root directory.

* title: The title of your presentation (displayed in the browser's title bar)
* reveal_theme: The reveal.js-theme to use [default.css]
* reveal_transition: The reveal.js-transition to use [default]
* reveal_theme_path: The path to the reveal.js-theme (can be changed for custom themes) [reveal.js/css/theme/]
* reveal_notes_server: Wether to support the speaker notes server [false (only local speaker notes)]
* reveal_options: Additional reveal.js [options][]
* reveal_dependencies: Additional reveal.js [dependencies][]
* reveal_path: Path to the reveal.js-installation [reveal.js]

### Multiple slides

To use multiple slides in one slide file, use a newline, three dashes and another newline like this:

    # Slide 1
    
    This is the content of Slide 1
    
    ---
    
    # Slide 2
    
    This is the content of Slide 2

### Vertical slides

To use vertical slides, do the same, but use two dashes:

    # Slide 1
    
    This is the content of Slide 1
    
    --
    
    And this is a vertical slide below Slide 1

### Fragments

Fragments allow slide elements to come one by one. This is often used in lists to subsequently show
fragments of a list during a presentation.

To use fragments, jekyll-reveal.js includes a jekyll-plugin, that simplifies the use of fragments
in markdown. To specify the current element as a fragment, use the {% fragment %}-tag like this:

    # Slide
    
    * This {% fragment %}
    * will {% fragment %}
    * come one by one {% fragment %}

### Slide backgrounds

To modify the background of the current slide, jekyll-reveal.js also includes a simplification
plugin:

    # Slide
    
    {% background white %}
    
    This slide has a white background

### Speaker notes

jekyll-reveal.js is configured, so that speaker notes are identified after an introductory "Note:"-tag:

    # Slide

    Some slide content

    Note:

    This is only displayed in the speaker notes.

[Reveal.js]:      http://lab.hakim.se/reveal-js/#/
[Jekyll]:         http://jekyllrb.com/
[Markdown]:       http://daringfireball.net/projects/markdown/ 
[example presentation]: http://dploeger.github.io/jekyll-revealjs/example
[install Jekyll]: http://jekyllrb.com/docs/installation/  
[options]: https://github.com/hakimel/reveal.js#configuration
[depedencies]: https://github.com/hakimel/reveal.js#dependencies

