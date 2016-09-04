# OPEN Kaposvár Hugo Theme

Our official website's theme based on the [Creative theme](//github.com/digitalcraftsman/hugo-creative-theme) by [@digitalcraftsman](//github.com/digitalcraftsman).

## Installation

Inside the folder of your Hugo site run:

    $ cd themes
    $ git clone https://github.com/openkaposvar/hugo-openkaposvar-theme

For more information read the official [setup guide](//gohugo.io/overview/installing/) of Hugo.


## Getting started

After installing the theme successfully it requires a just a few more steps to get the site running.


### The config file

Take a look inside the [`exampleSite`](//github.com/openkaposvar/hugo-openkaposvar-theme/tree/master/exampleSite) folder of this theme. You'll find a file called [`config.toml`](//github.com/openkaposvar/hugo-openkaposvar-theme/blob/master/exampleSite/config.toml).

To use it, copy the [`config.toml`](//github.com/openkaposvar/hugo-openkaposvar-theme/blob/master/exampleSite/config.toml) in the root folder of website. Feel free to change strings as you like to customize the website.


### Change the hero background

The hero acts as an eye-catcher for the site. So consider to give him a nice background. You just need to replace the [`header.jpg`](//github.com/openkaposvar/hugo-openkaposvar-theme/blob/master/static/img/header.jpg) at [`static/img`](//github.com/openkaposvar/hugo-openkaposvar-theme/tree/master/static/img) with your own. But it's important that you use the same filename.


### Add your services

This section should show your capabilities and skills. You can change the services under  at `[params.services.list]` in the [`config.toml`](//github.com/digitalcraftsman/hugo-creative-theme/blob/dev/exampleSite/config.toml).

All icons using Fontawesome's icon font. Look at the website of [Fontawesome](//fortawesome.github.io/Font-Awesome/icons/) for more icons. The icons are represented by their corresponding CSS class. A skill is defined like this example:

```toml
[[params.services.list]]
    icon = "fa-diamond"
    title = "Sturdy Templates"
    description = "Our templates are updated regularly so they don't break."
```

### Create your portfolio

Beside the config file, there is in `data` another subfolder called [`projects`](//github.com/digitalcraftsman/hugo-creative-theme/tree/master/exampleSite/data/projects) which hosts the files that will appear as your projects in the portfolio section. Such a project file might look like [this one](//github.com/digitalcraftsman/hugo-creative-theme/blob/dev/exampleSite/data/projects/2014-07-05-project-1.yaml) written in YAML:

```yaml
modalID: 1
title: Project 1
date: 2014-07-05
img: 1.jpg
client: Start Bootstrap
clientLink: "#"
category: Web Development
description: Lorem ipsum dolor sit amet, consectetur adipisicing elit. Vel enim aliquid dicta ullam in repellendus amet perspiciatis adipisci architecto obcaecati sit voluptas ipsam, deleniti neque placeat tenetur cum tempore velit.
```

Copy the folder [`projects`](//github.com/openkaposvar/hugo-openkaposvar-theme/tree/master/exampleSite/data/projects) inside the `data` folder in the **root** directory of your site. Let's make some changes to show your work.

Pay attention to the `modalID`. It must be a unique integer and be incremented with each new project you want to add to the portfolio. Otherwise, the corresponding modal can't be rendered.

Furthermore, you can use Markdown syntax for URLs like here `[text](//url.to/source)` in the description.

To give your projects an image, save those under [`static/img/portfolio`](//github.com/openkaposvar/hugo-openkaposvar-theme/tree/master/static/img/portfolio). The dimensions should be 650 x 350 pixels. Don't forget to set the **filename** under 'img' in your project.


### Nearly finished

In order to see your site in action, run Hugo's built-in local server. 

    $ hugo server

Now enter [`localhost:1313`](https://localhost:1313) in the address bar of your browser.


## Contributing

Did you found a bug or got an idea for a new feature? Feel free to use the [issue tracker](//github.com/openkaposvar/hugo-openkaposvar-theme/issues) to let me know. Or make directly a [pull request](//github.com/openkaposvar/hugo-openkaposvar-theme/pulls).

Please create a separate branch for your pull request.


## License

This theme is released under the Apache License 2.0 For more information read the [license](//github.com/openkaposvar/hugo-openkaposvar-theme/blob/master/LICENSE).


## Acknowledgements

Thanks to 

- [Steve Francia](//github.com/spf13) for creating Hugo and the awesome community around the project
- [David Miller](//github.com/davidtmiller) for creating the original Bootstrap theme
- [digitalcraftsman](//github.com/digitalcraftsman) for creating the original Hugo theme
