# Ghostcraft - ghost theme boilerplate

> A [Ghost](https://ghost.org/) theme focused on content

### [→ Download](https://github.com/pixel-craft/ghostcraft/archive/master.zip)


## Table of contents

* [Features](#features)
* [Installing](#installing)
* [Configuring](#configuring)
* [License](#license)

## Features

* Content first
* Fully responsive
* HTML5 semantics, WAI-ARIA and Rich Snippets roles (json)
* Disqus comments integration
* Google Universal Analytics snippet
* OpenGraph and Twitter Cards meta's
* Baseline HTML5 features responsive meta
* One-file CSS for performance
* Minify css

## Installing

### Using Git
1. Navigate to your Ghost theme directory `ghost/content/themes`
2. Clone the theme repository using the command below
```sh
$ git clone https://github.com/pixel-craft/ghostcraft/
```
3. Restart ghost and log in to your dashboard
4. In settings under themes select **ghostcraft** and save
5. That's all, now its time to [configure](#configuring) your theme


### Manually
1. Download the files using the [GitHub .zip download](https://github.com/pixel-craft/ghostcraft/archive/master.zip) option
2. Unzip the files and rename the folder to `ghostcraft`
4. Copy the folder into your Ghost theme directory `ghost/content/themes`
5. Restart ghost and log in to your dashboard
6. In settings under themes select **ghostcraft** and save
7. That's all, now its time to [configure](#configuring) your theme

## Configuring

### Comments

You can add your disqus URL  in **comments.hbs** file in `/partials/custom/comments.hbs`.

Delete {{> custom/comments}} in **post.hbs** if you don't use comment on your website.

### Email / contact

You can add your email with mailto  in **follow.hbs** file in `/partials/custom/follow.hbs`. It's better to hash it in order to avoid spam.

### meta.hbs

All configurable meta are located in `/partials/custom/meta.hbs`.

* Theme color on mobile
* Custom favicon (based on favomatic)
 * **favicon.ico is at the root of the folder**
* Windows application tiles

### Analytics

You can add google analytics code or another tracking tool with the code injection in Settings.

### Editing Follow Buttons and email

This THEME is based on Font Awesome for icons.
See the Font Awesome documentation for the [full list of icons](http://fortawesome.github.io/Font-Awesome/icons/).

You can customize the icons of the header in **follow.hbs** file in `/partials/custom/follow.hbs`.

Make sure to replace the `username` in the URLs so the links point to your profiles. Or delete the useless profiles.

	If you want to add an email / it's better to hash it
	<a href="mailto:you@example.com"><i class="fa fa-envelope-square fa-2x"></i></a>

	<a href="http://github.com/username"><i class="fa fa-github-square fa-2x"></i></a>
	<a href="http://plus.google.com/+username"><i class="fa fa-google-plus-square fa-2x"></i></a>
	<a href="http://instagram.com/username"><i class="fa fa-instagram fa-2x"></i></a>
	<a href="http://vimeo.com/username"><i class="fa fa-vimeo-square fa-2x"></i></a>
	<a href="http://youtube.com/username"><i class="fa fa-youtube-square fa-2x"></i></a>
	<a href="http://flickr.com/username"><i class="fa fa-flickr fa-2x"></i></a>
	<a href="http://pinterest.com/username"><i class="fa fa-pinterest-square fa-2x"></i></a>
	<a href="http://username.tumblr.com"><i class="fa fa-tumblr-square fa-2x"></i></a>

### Design
The css structure is base on BEM and atom design systems.

Use the **__dev** folder to create your css cascade.

## License

[MIT License](http://oswaldoacauan.mit-license.org/) © Oswaldo Acauan
