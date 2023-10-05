# PaperSite Template

[![Hugo](https://img.shields.io/badge/hugo-0.88-blue.svg)](https://gohugo.io)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

### [Hugo](https://gohugo.io) theme for scientific projects

- [Requirements](#requirements)
- [Installation](#installation)
- [Configuration](#configuration)
- [Shortcodes](#shortcodes)

## Requirements

- Hugo 0.79 or higher
- Hugo extended version, read more [here](https://gohugo.io/news/0.48-relnotes/)

## Installation

### Install as git submodule
Navigate to your hugo project root and run:

```
git submodule add https://github.com/Tr4mper/papersite-template themes/papersite-template
```

Then run hugo (or set `theme = "papersite-template"`/`theme: papersite-template` in configuration file)

```
hugo server --minify --theme papersite-template
```

### Try out the example

```
hugo server --source=exampleSite --themesDir=../..
```

### Creating site from scratch

Below is an example on how to create a new site from scratch:

```sh
hugo new site mydocs; cd mydocs
git init
git submodule add https://github.com/alex-shpak/hugo-book themes/hugo-book
cp -R themes/papersite-template/exampleSite/content.en/* ./content
```

```sh
hugo server --minify --theme hugo-book
```