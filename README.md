# GDPR Child Theme

This is a WordPress child theme boilerplate, which aims to secure the site and to configure it to meet the GDPR requirements. The child theme performs the following tasks:

* Localize Google Fonts (or in fact any web font)
* Make links in the comments truely external
* Remove the commentor's IP (old ones have to be removed by hand)
* Disable oEmbeds (old ones have to be removed by hand)
* Disable WordPress Emojis (in every modern browser Emojis will be displayed anyway)
* Remove global DNS Prefetching
* Hide WordPress REST API for security reasons

## Instructions

This is a child theme is a boilerplate! If you want to create your own child theme for any  WordPress theme, please fork or clone this repository and change the `gdpr_` prefix in the `functions.php` to your own theme name.

Not every parent theme works the same. You may have to change the code in the `gdpr_child_enqueue_scripts()` so that it's working properly.

### CSS

In order to create clean code and a descent inheritance, the child theme uses a `.child` body class once you activated the child theme. If you want to append your own CSS code to the `style.css`, you should use this class as a prefix, e.g.:

```css
.child p {
  line-height: 1.6
}
```

### Fonts

If you want to localize Google Fonts, simply use the [google-webfonts-helper](https://google-webfonts-helper.herokuapp.com/fonts), copy the downloaded fonts to the `/fonts/` directory and edit the `/css/fonts.css`.

**NOTE:** To use the `TODO` file you should edit it with VSCode and the `Todo+` extension. Please read their documentation for usage information.