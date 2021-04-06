
<p align="center"><img align="center" width="350" src="https://raw.githubusercontent.com/arturo-lang/autom8/master/logo.png"/></p>
<p align="center">
  <b>Fast templating<br>for any type of project</b>
  <br><br>
  <img src="https://img.shields.io/github/license/arturo-lang/autom8?style=for-the-badge">
  <img src="https://img.shields.io/badge/language-Arturo-orange.svg?style=for-the-badge">
<!--  <img src="https://img.shields.io/github/workflow/status/arturo-lang/grafito/Run%20Tests?style=for-the-badge">-->
</p>

<!--<p align="center"><img width="90%" align="center" src="https://raw.githubusercontent.com/arturo-lang/grafito/master/screenshot.png"/></p>-->

---

<!--ts-->

* [At A Glance](#at-a-glance)
* [Try Autom8](#try-autom8)
    * [Pre-built binaries](#pre-built-binaries)
    * [Installation](#installation)
        * [As a Library](#as-a-library)
        * [As a Standalone tool](#as-a-standalone-tool)
* [Community](#community)
* [License](#license)   

<!--te-->
 
---

## At A Glance

Let's dive into some Autom8 script (yep, that is all you need to set it up!):

```red
; Sample project
; for converting a series of User data files
; into HTML pages

verbose: true

rules: [
    ".art$" # [
        title: "Processing files"

        target:   $[f][append f -- extract.extension f ".html"]
        template: "template.html"
    ]
]
```

## Try Autom8!

<img align="center" src="https://raw.githubusercontent.com/arturo-lang/autom8/master/docs/sketch.png"/>

### Pre-built binaries

Autom8 already comes in ready-to-run binaries for Linux & macOS (more on the way).

Feel free to check out the [Releases](https://github.com/arturo-lang/autom8/releases) section yourself!

### Installation

To install local, first you have to have installed the latest version of [Arturo](https://github.com/arturo-lang/arturo).

Then, just clone this repo and simply go to the folder via your terminal.


#### As a Library

After having installed the latest version of Arturo, you can use Autom8 from any Arturo script as a library.

#### As a Standalone tool

Of course, you can also run Autom8 as a tool on it own:

```
autom8 <file path> (--at:destination) (--config:configuration)
```


Community
------------------------------

In case you want to ask a question, suggest an idea, or practically anything related to Autom8 (or Arturo) - feel free! Everything and everyone is welcome.

For that, the most convenient place for me would be the [GitHub Issues](https://github.com/arturo-lang/autom8/issues) page.

[![Stargazers over time](https://starchart.cc/arturo-lang/autom8.svg)](https://starchart.cc/arturo-lang/autom8)

## License

MIT License

Copyright (c) 2021 Yanis Zafirópulos

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
