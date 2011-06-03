=== WP Display Header ===
Contributors: kobenland
Tags: admin, custom header, header, header image, custom header image, display header, display dynamic header
Donate link: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=MWUA92KA2TL6Q
Requires at least: 3.0
Tested up to: 3.2-beta
Stable tag: 1.3

Select a specific header or random header image for each content item.

== Description ==

This plugin lets you specify a header image for each post individually from your default headers and custom headers.

It adds a meta box in the post edit screens with the header selection.
If no specific header is specified for a post it will fall back to the default selection.
There is no change of template files necessary as this plugin hooks in the existing WordPress API to unfold its magic.


= Translations =
I will be more than happy to update the plugin with new locales, as soon as I receive them!
Currently available in:

* English
* Deutsch
* Italiano

Thanks to Erik T. for the idea to this plugin!

== Installation ==

1. Download WP Display Header.
2. Unzip the folder into the `/wp-content/plugins/` directory
3. Activate the plugin through the 'Plugins' menu in WordPress


== Frequently Asked Questions ==

None asked yet.

= Plugin Filter Hooks =

**wpdh_show_default_header** (*bool*)
> Whether to show the default header (true) or to look for a specifically selected header for the current request.

**wpdh_get_header_posts** (*array*)
> All attachments with the meta key `_header_image`. An array with the query vars.

**wpdh_get_headers** (*array*)
> The array with all registered headers.

**wpdh_get_active_post_header** (*string*)
> The url to the currently active header image.


== Screenshots ==

1. The meta box in the main column.
2. The meta box in the side column.


== Changelog ==

= 1.3 =
* Tested for WordPress 3.2-beta
* Fixed a minor bug where a PHP warning was issued in the edit-post-screen, when there are no header images registered.

= 1.2.1 =
* WordPress Plugin Repository update bug

= 1.2 =
* Tested for WordPress 3.1.2
* Now a custom folder name can be specified. See: Settings > Media
* Added Italian translation (Thanks to Pietro Rossi)

= 1.1 =
* Tested for WordPress 3.1.1
* Adopted [WP Save Custom Header](http://wordpress.org/extend/plugins/wp-save-custom-header/ "This plugin lets you save and reuse your uploaded header images.") multisite capability
* Made HTML W3C valid

= 1.0 =
* Initial Release