# hugo-shortcodes
Single shortcodes for Hugo may come handy when building a website

## icon.html

Super-simple shortcode, mainly useful with a icon library like [Font Awesome](https://fontawesome.com/).

You can use these icons freely within the Hugo markdown content files.

### Usage

The shortcode is using several parameter:

* iconClass - Style used for the \<i> element, place here your Font Awesome styles.
* link - URL, if you want your icon to be a hyperlink.
* linkClass - Style used for the \<a> element when link-parameter is in use.   
* style - Additional inline style.

### Examples

```
{{<icon iconClass="fas fa-envelope fa-3x" linkClass="email" style="margin-right: 50px;">}}
```

```
{{<icon iconClass="fas fa-envelope fa-3x" linkClass="email" style="margin-right: 50px;" link="mailto://">}}
```

