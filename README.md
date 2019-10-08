# hugo-shortcodes
Single shortcodes for Hugo may come handy when building a website.

## icon.html

Super-simple shortcode, mainly useful with a icon library like [Font Awesome](https://fontawesome.com/).

You can use these icons freely within the Hugo markdown content files.

### Usage

The shortcode is using several parameter:

* iconClass - String, Style used for the \<i> element, place here your Font Awesome styles.
* link - String, The URL if you want your icon to be a hyperlink.
* linkClass - String, Style used for the \<a> element when link-parameter is in use.
* style - String, Additional inline style.

### Examples

```
{{<icon iconClass="fas fa-envelope fa-3x" linkClass="email" style="margin-right: 50px;">}}
```

```
{{<icon iconClass="fas fa-envelope fa-3x" linkClass="email" style="margin-right: 50px;" link="mailto://">}}
```

## img.html

Supports featherlight box and Hugo's image processing features. Featherlight must be available with your site/theme.

### Usage

The shortcode is using several parameter:

* src - String, image URL.
* cmd - String, "COMMAND OPTION" Command must be either "Fill", "Resize" or "Fit" with appropriate options, see [Image Processing Methods](https://gohugo.io/content-management/image-processing/#image-processing-methods).
* box - Bool, Use "true" if featherlight box should be used.

### Examples

```
{{<img src="image.jpg" box="true" command="Resize 800x" >}}
```

```
{{<img src="image.jpg" command="Fill 800x640 Center" >}}
```

### ToDo

- [ ] Support for filters supported since Hugo 0.58
