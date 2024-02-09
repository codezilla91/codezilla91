# Universal Theme for Hugo

Universal is a clean and stylish website template built with [Bootstrap](https://getbootstrap.com/docs/3.4/getting-started/). It stands out with its clean design and elegant typography.

Demo site: [https://devcows.github.io/hugo-universal-theme](https://devcows.github.io/hugo-universal-theme/)

Sponsor this project:

- [https://paypal.me/ryanfox1985](https://paypal.me/ryanfox1985)
- [https://www.patreon.com/ryanfox1985](https://www.patreon.com/ryanfox1985)

This Hugo theme was ported from [Bootstrapious](http://bootstrapious.com/p/universal-business-e-commerce-template) for training and fun. It has a very nice and customizable landing page, a comments system by Disqus, site search by Google, contact forms by Formspree, Google Analytics, and optional widgets for the sidebar.

![screenshot](https://raw.githubusercontent.com/devcows/hugo-universal-theme/master/images/screenshot.png)

## Table of Contents

- [Universal Theme for Hugo](#universal-theme-for-hugo)
  - [Table of Contents](#table-of-contents)
  - [Features](#features)
  - [Installation](#installation)
  - [Configuration](#configuration)
    - [Language](#language)
    - [Style](#style)
    - [Comments](#comments)
    - [Google Analytics](#google-analytics)
    - [Logo](#logo)
    - [Contact form](#contact-form)
    - [Menu](#menu)
    - [Sidebar widgets](#sidebar-widgets)
    - [Top bar](#top-bar)
    - [Blog post thumbnails](#blog-post-thumbnails)
    - [Landing page](#landing-page)
      - [Carousel](#carousel)
      - [Features](#features-1)
      - [Testimonials](#testimonials)
      - [See more](#see-more)
      - [Clients](#clients)
      - [Recent posts](#recent-posts)
      - [Footer](#footer)
        - [About us](#about-us)
        - [Recent posts](#recent-posts-1)
        - [Contact](#contact)
    - [Meta tags](#meta-tags)
  - [Usage](#usage)
  - [Contributing](#contributing)
  - [License](#license)
  - [Thanks](#thanks)

## Features

- Responsive design
- Customizable landing page
  - Carousel
  - Testimonials
  - Features
  - Customers
  - Recent posts
- Contact form by Formspree
- Google search
- Disqus comments
- Google Analytics

## Installation

Go to the directory where you have your Hugo site and run:

```
$ mkdir themes
$ cd themes
$ git clone https://github.com/devcows/hugo-universal-theme
```

For more information read the official [setup guide](https://gohugo.io/installation/) of Hugo.

## Configuration

After installing the Universal theme successfully, we recommend you to take a look at the [exampleSite](//github.com/devcows/hugo-universal-theme/tree/master/exampleSite) directory. You will find a working Hugo site configured with the Universal theme that you can use as a starting point for your site.

First, let's take a look at the [config.toml](//github.com/devcows/hugo-universal-theme/tree/master/exampleSite/config.toml). It will be useful to learn how to customize your site. Feel free to play around with the settings.

### Language

Available translations are in the `/i18n` directory. You can configure the language modifying the following key.

```toml
defaultContentLanguage = "en"
```

### Style

You can change the color of the theme by modifying the following key.

```toml
style = "default"
```

Available options are: `default` (light-blue), `blue`, `green`, `marsala`, `pink`, `red`, `turquoise`, `violet`.
There is the possibility to override the CSS and set your custom styles, override this file `static/css/custom.css` in your site.

### Comments

The optional comments system is powered by [Disqus](https://disqus.com). If you want to enable comments, create an account in Disqus and write down your shortname.

```toml
disqusShortname = "devcows"
```

You can disable the comments system by leaving the `disqusShortname` empty.

### Google Analytics

You can optionally enable Google Analytics. Type your tracking code in the ``.

```toml
googleAnalytics = "UA-XXXXX-X"
```

Leave the `googleAnalytics` key empty to disable it.

### Logo

A logo can be selected, two parameters `logo` and `logo_small` can be defined. By default `logo` is used for medium and big screens and the `logo_small` value will be used when the site is rendered on small screens. Also there is the possibility to disable the logo and render a alternative text.

```toml
[params]
    disabled_logo = false
    logo_text = "Universal"

    logo = "img/logo.png"
    logo_small = "img/logo-small.png"
```

### Contact form

You can optionally create a contact page and include a contact form.

A contact page is just like a regular Hugo page. But it must include the field `id` with the value `contact`.

```toml
+++
title = "Contact"
id = "contact"
+++
```
# codezilla91
