=== Catch Gallery ===
Contributors: catchplugins, catchthemes, sakinshrestha, pratikshrestha, maheshmaharjan, dreamsapana
Donate link: https://catchplugins.com/plugins/catch-gallery/
Tags: gallery, tiled gallery, image gallery, mosaic, carousel, lightbox, media, jetpack, jetpack lite
Requires at least: 5.9
Requires PHP: 7.4
Tested up to: 7.0
Stable tag: 3.0
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Catch Gallery allows you to add three different types of layouts (in addition to the default layout provided by WordPress – Thumbnail Grid) for your galleries to stand out—Tiled Mosaic, Square Tiles, Circles.

== Description ==

Catch Gallery - a simple gallery plugin for WordPress helps you create stunning galleries. Catch Gallery was inspired by the Jetpack’s Gallery Module. With Catch Gallery, you will be able to exhibit outstanding galleries and portfolios on your creative WordPress websites. It is extremely easy to use. The plugin carries a completely responsive design and your galleries will look appealing from any device. With our new gallery plugin, you can effortlessly boost your website's appearance, giving it the A-class look that it deserves. Catch gallery allows you to enable and choose the background color of the carousel, show photo metadata, comments, and view full-size images in the gallery. Catch Gallery allows you to add three different types of layouts (in addition to the default layout provided by WordPress – Thumbnail Grid) for your galleries to stand out—Tiled Mosaic, Square Tiles, Circles. These attractive layouts are sure to bring your galleries to life and make it more elegant and appealing. Catch Gallery is extremely lightweight, comes with responsive design, and compatible with all themes. Download Catch Gallery and make your galleries more appealing!

Demo Tiled Gallery :  [Demo link](https://catchplugins.com/demo/?data=b3BEbnJ1ZVpocXoxU0hvYXFLaGlWUT09 "Demo Link")

Plugin Instructions :  [Instructions link](https://catchplugins.com/plugins/catch-gallery/#instructions "Instructions Link")

== Screenshots ==

1. Main Page
2. Create Gallery in Page/Post Step 1
3. Gallery Settings - Select Type
4. Type: Tiled Mosaic Layout
5. Type: Square Tiles Layout
6. Type: Circles Layout

== Installation ==

The easy way (via Dashboard) :

* Go to Plugins > Add New
* Type in the **Catch Gallery** in Search Plugins box
* Click Install Now to install the plugin
* After Installation click activate to start using the **Catch Gallery**
* Go to **Catch Gallery** from Dashboard menu

Not so easy way (via FTP) :

* Download the **Catch Gallery**
* Unarchive **Catch Gallery** plugin
* Copy folder with catch-infinite-scroll.zip
* Open the ftp \wp-content\plugins\
* Paste the plug-ins folder in the folder
* Go to admin panel => open item "Plugins" => activate **Catch Gallery**
* Go to **Catch Gallery** from Dashboard menu

For Detailed Plugin instructions, checkout Instructions tab at https://catchplugins.com/plugins/catch-gallery/#instructions

== Changelog ==

= 3.0 (Released: May 21, 2026) =
* Bug Fixed: Settings page capability changed from 'edit_posts' to 'manage_options' — only administrators should be able to modify global gallery settings
* Bug Fixed: Inverted nonce logic in catch_gallery_sanitize_callback() — was saving data on nonce failure and returning 'Invalid Nonce' string on success, corrupting saved settings
* Bug Fixed: Carousel Background Color dropdown always showed no selection — both <option> elements compared against 'scroll' instead of 'black'/'white'
* Bug Fixed: Unsanitized $_POST inputs in post_attachment_comment() — added sanitize_textarea_field(), sanitize_text_field(), sanitize_email(), esc_url_raw() and wp_unslash()
* Bug Fixed: Missing wp_verify_nonce() unslash in post_attachment_comment()
* Bug Fixed: Unescaped $img_src['url'] in square_talavera() — wrapped with esc_url()
* Bug Fixed: Unescaped $ctp_options output in catch-gallery-display.php — wrapped with esc_attr()
* Bug Fixed: wptexturize() caption output not escaped — wrapped with wp_kses_post()
* Bug Fixed: json_encode() in HTML attributes replaced with esc_attr( wp_json_encode() ) in tiled-gallery.php and jetpack-carousel.php
* Bug Fixed: die(json_encode()) and header() patterns replaced with wp_send_json() / wp_send_json_error() in jetpack-carousel.php
* Bug Fixed: Missing error check after wp_get_image_editor()->save() in vt_resize() — now returns original image on failure
* Bug Fixed: extract() replaced with explicit variable assignments in get_attachments()
* Bug Fixed: Missing wp_parse_args() in catch_gallery_get_options() — new default options were not applied to existing installations
* Bug Fixed: Missing version number on tiled-gallery script enqueue causing browser cache issues
* Bug Fixed: Duplicate wp_get_attachment_url() call in generate_carousel_image_args() — reuses already-fetched $orig_file
* Bug Fixed: Wrong @package annotation in display-dashboard.php — was 'Catch_Ids', corrected to 'Catch_Gallery'
* Bug Fixed: Typo 'Tiled Mosiac' corrected to 'Tiled Mosaic' in features tab
* Bug Fixed: Loose null == comparison changed to strict null === in catch_gallery_default_options()
* Bug Fixed: __() changed to esc_html__() in core_media_widget_compat() schema description
* Bug Fixed: Raw HTML in plugin meta links row wrapped with wp_kses()
* Bug Fixed: IE8 conditional stylesheet removed — IE8/IE9 no longer supported by WordPress
* Bug Fixed: include() changed to require_once for critical plugin files in catch-gallery.php
* Updated: Minimum Requires PHP to 7.4
* Compatibility check up to version 7.0

= 2.4.1 (Released: February 25, 2026) =
* Bug Fixed: Fixed JS enqueue path for adding catch themes tab item in Themes add theme section
* Bug Fixed: Fixed error occurred while adding new themes

= 2.4 (Released: February 02, 2026) =
* Bug Fixed: WordPress.WP.I18n.MissingTranslatorsComment
* Bug Fixed: WordPress.WP.I18n.MissingArgDomain
* Bug Fixed: WordPress.WP.I18n.TextDomainMismatch
* Bug Fixed: plugin_header_invalid_author_uri
* Bug Fixed: WordPress.Security.EscapeOutput.OutputNotEscaped
* Bug Fixed: WordPress.WP.AlternativeFunctions.parse_url_parse_url
* Bug Fixed: WordPress.Security.NonceVerification.Recommended
* Bug Fixed: WordPress.Security.ValidatedSanitizedInput.InputNotValidated

= 2.3 (Released: January 07, 2026) =
* Compatibility check up to version 6.9

= 2.2 (Released: May 27, 2025) =
* Bug Fixed: Image loading issue for tiled mosaic

= 2.1 (Released: May 12, 2025) =
* Compatibility check up to version 6.8

= 2.0 (Released: November 15, 2023) =
* Compatibility check up to version 6.4

= 1.9 (Released: November 03, 2022) =
* Compatibility check up to version 6.1

= 1.8 (Released: February 24, 2022) =
* Compatibility check up to version 5.9

= 1.7 (Released: September 16, 2021) =
* Bug Fixed: Security issue on ajax calls

= 1.6.8 (Released: July 23, 2021) =
* Bug Fixed: hover event replaced by mouseenter and mouseleave, deprecated as of jQuery 1.8
* Compatibility check up to version 5.8

= 1.6.7 (Released: May 04, 2021) =
* Updated: CSS breakpoints for better responsiveness

= 1.6.6 (Released: April 21, 2021) =
* Bug Fixed: Gallery Responsive issue

= 1.6.5 (Released: March 04, 2021) =
* Bug Fixed: Deprecate required parameters after optional parameters in function/method signatures
* Compatibility check up to version 5.7

= 1.6.4 (Released: August 28, 2020) =
* Added: Title attribute on images

= 1.6.3 (Released: August 19, 2020) =
* Bug Fixed: Issue in add new theme page

= 1.6.2 (Released: August 11, 2020) =
* Update: Default image size set to full
* Compatibility check up to version 5.5

= 1.6.1 (Released: April 09, 2020) =
* Bug Fixed: Undefined index issue in tiled gallery

= 1.6 (Released: April 08, 2020) =
* Fixed: Ability to change column and image sizes

= 1.5 (Released: March 10, 2020) =
* Compatibility check up to version 5.4

= 1.4 (Released: November 12, 2019) =
* Compatibility check up to version 5.3

= 1.3 (Released: August 20, 2019) =
* Added: Tooltip for info icons
* Added: Option to turn off Catch Themes and Catch Plugins tabs
* Compatibility check up to version 5.2
* Updated: Catch Themes and Catch Plugins tabs displaying code

= 1.2 (Released: February 21, 2019) =
* Compatibility check up to version 5.1

= 1.1 (Released: 12 December, 2018)=
* Added: Catch Themes and Catch Plugins tabs in Add themes and Add plugins page respectively
* Added: Themes by Catch Themes section under Themes panel in customizer
* Compatibility check up to version 5.0

= 1.0.1 (Released: 05 June, 2018)=
* Bug Fixed: Gallery Widget now saves plugins options

= 1.0 (Released: 04 June, 2018)=
* Initial Release
