# Lens

Lens is a full screen responsive photo gallery, featuring a completely full screen experience. It is a port of [Lens](//html5up.net/lens) by [HTML5 UP](//html5up.net).

![Hugo Lens Theme screenshot](https://raw.githubusercontent.com/christianmendoza/hugo-lens-theme/master/images/screenshot.png)


## Demo

Demo available on [cm-hugo-lens-theme.firebaseapp.com](//cm-hugo-lens-theme.firebaseapp.com/).


## Installation

Inside the folder of your Hugo site run:

    $ cd themes
    $ git clone https://github.com/christianmendoza/hugo-lens-theme

For more information read the official [setup guide](//gohugo.io/overview/installing/) of Hugo.


## Getting started

After installing the Lens theme successfully it requires a just a few more steps to get your site finally running.


### The config file

Take a look inside the [`exampleSite`](//github.com/christianmendoza/hugo-lens-theme/tree/master/exampleSite) folder of this theme. You'll find a file called [`config.toml`](//github.com/christianmendoza/hugo-lens-theme/blob/master/exampleSite/config.toml). To use it, copy the [`config.toml`](//github.com/christianmendoza/hugo-lens-theme/blob/master/exampleSite/config.toml) in the root folder of your Hugo site. Feel free to customize this theme as you like.


### Example demo

In the [`exampleSite`](//github.com/christianmendoza/hugo-lens-theme/blob/master/exampleSite) folder you can find an example [`data`](//github.com/christianmendoza/hugo-lens-theme/blob/master/exampleSite/data) folder with a `data.toml` file and [`static`](//github.com/christianmendoza/hugo-lens-theme/blob/master/static). Copy both folders to the root folder of your Hugo site. Start/restart your local server to see an example site with a few test placeholder images.


### Add new images

Data for all images is stored in `data/data.toml`. Upload full and thumbnail size images to your `static` folder in any folder structure you wish. Use the following snippet below to add new images.

```toml
[[images]]
  title = "Diam tempus accumsan"
  caption = "Lorem ipsum dolor sit amet, consectetur adipiscing elit."
  imagePathFull = "images/fulls/01.jpg"
  imagePathThumb = "images/thumbs/01.jpg"
  position = "left center"
```

Each image has a `title` and `caption` text. Update both `imagePathFull` and `imagePathThumb` accordingly to where you saved your images. `position` corresponds to how the image will be displayed in the main viewer. It's centered by default, however you can have a specific area be shown by supplying a valid css background position value.


### Keyboard shortcuts

Lens is set up to respond to the following keyboard shortcuts:

- Left Arrow: Go to previous image.
- Right Arrow: Go to next image.
- Up Arrow: Go to image above the current one in the thumbnails section.
- Down Arrow: Go to image below the current one in the thumbnails section.
- Space: Go to next image.
- Escape: Toggle the main wrapper.

Note: All keyboard shortcuts are disabled when the "xsmall" breakpoint is active (since they don't really make a whole lot of sense there).


### Additional settings

There are additional settings you can configure which are located in the [`static/assets/js/main.js`](//github.com/christianmendoza/hugo-lens-theme/blob/master/static/assets/js/main.js) file.

```
settings: {

  // Preload all images.
  preload: false,

  // Slide duration (must match "duration.slide" in _vars.scss).
  slideDuration: 500,

  // Layout duration (must match "duration.layout" in _vars.scss).
  layoutDuration: 750,

  // Thumbnails per "row" (must match "misc.thumbnails-per-row" in _vars.scss).
  thumbnailsPerRow: 2,

  // Side of main wrapper (must match "misc.main-side" in _vars.scss).
  mainSide: 'right'

}
```

The above are all default. Take note that most changes will require you to edit the sass file [`static/assets/sass/libs/_vars.scss`](//github.com/christianmendoza/hugo-lens-theme/blob/master/static/assets/sass/libs/_vars.scss) and recompile the css to the [`static/assets/css`](//github.com/christianmendoza/hugo-lens-theme/blob/master/static/assets/css) folder. 


### Add social icon links

Add icons to your social media properties. Change `label`, `icon`, and `url` accordingly. Follow the same snippet to add more icon links. Remove any of those you don't want.

```toml
[[params.social]]
  label = "Twitter"
  icon = "fa-twitter"
  url = "#"
```


### Add Google Analytics

Enable Google Analytics by adding your tracking id to `googleAnalytics`. Leave empty or remove if you don't want.

```toml
googleAnalytics = "UA-XXXXXXXX-1"
```


### Nearly finished

In order to see your site in action, run Hugo's built-in local server.

    $ hugo server

Now enter [`localhost:1313`](http://localhost:1313) in the address bar of your browser.


## Contributing

Did you found a bug or got an idea for a new feature? Feel free to use the [issue tracker](//github.com/christianmendoza/hugo-lens-theme/issues) to let me know. Or make directly a [pull request](//github.com/christianmendoza/hugo-lens-theme/pulls).


## License

The original template is released under the [Creative Commons Attribution 3.0 License](//github.com/christianmendoza/hugo-lens-theme/blob/master/LICENSE.md). Please keep the original attribution link when using for your own project. If you'd like to use the template without the attribution, you can check out the license option via the template [author's website](//html5up.net/lens).


## Annotations

- Original [Lens](//html5up.net/lens) Template by [HTML5 UP](//html5up.net)

Also thanks to [Steve Francia](//github.com/spf13) for creating [Hugo](//gohugo.io) and the awesome community around the project.
