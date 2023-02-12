# `tableofcontents` Extension For Quarto `revealjs` Format

A plugin for [Reveal.js](https://github.com/hakimel/reveal.js) allowing some options regarding creation of table of contents, such as putting table of contents at an arbitrary slide, stepping through the elements of table of contents etc.

## Installing

``` bash
quarto add shafayetShafee/tableofcontents
```

This will install the extension under the `_extensions` subdirectory. If you're using version control, you will want to check in this directory.

## Usage

Simply add the extension to the list of reveal plugins like:

``` yaml
format: revealjs
tableofcontents:
  # set tableofcontents configuration options here
revealjs-plugins:
  - tableofcontents
```

## Options

You can pass the following options to `tableofcontents`

| Option             | Description                                                                                                                                |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------|
| `title`            | Specifies the slide title of the table of contents slide. Default is `"Table of Contents"`.                                                |
| `titleTag`         | Specifies html tag in which the table of contents title stands. Default is `"h1"`.                                                         |
| `position`         | Specifies the position of the table of contents slide in the presentation. Default is `2`.                                                 |
| `titleTagSelector` | Specifies which slide tag elements will be used for generating the table of contents. Default is `h1, h2, h3, h4, h5, h6"`.                |
| `ignoreFirstSlide` | Specifies whether title slide's title should be ignored in table of contents. Default is `true`.                                           |
| `fadeInElements`   | Specifies if every single element of the table of contents will be stepped through before moving on to the next slide. Default is `false`. |


## Example

Here is the source code for a minimal example: [example.qmd](example.qmd) and the [rendered output](https://shafayetshafee.github.io/tableofcontents/example.html)

------------------------------------------------------------------------

[reveal.js-tableofcontents - Reveal.js Plugin](https://github.com/naamor/reveal.js-tableofcontents) by Roman Stocker ([\@naamor](https://github.com/naamor)) under MIT License.
