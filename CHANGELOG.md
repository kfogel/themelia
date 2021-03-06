Change Log
==========

All notable changes to Themelia will be documented in this file. This changelog adheres to [Semantic Versioning](http://semver.org/). Version format will look like `3.2.1` where `3` is the major release, `2` is the minor release, and `1` is the patch release.

v1.2.2 - 2018-01-03
--------------------

### Fix

-	Minor CSS improvements, clearing floats.

v1.2.1 - 2017-12-22
--------------------

### Fix

-	Title output on archive page - fixed missing whitespace between month and year. Tnx `@getnaked`.

### Updated

-	Changed Text Domain in Hybrid Core library to 'themelia'.

v1.2.0 - 2017-11-19
--------------------

### Updated

-	Compatibility with WP version 4.9 is 100%.
-   HybridCore library is updated to version 4.0. One of the changes in 4.0 is that the framework no longer defines Schema.org as a default. It leaves this up to theme authors. Additionally, it only sets defaults for the body, post, and comment attributes. Themelia has Schema.org defined and attributes for all elements are re-added. The change is in the `functions-attr.php` file. Developers, see what's new in HybridCore branch 4 `library\changelog.md`.
-   Kirki library is updated to version 3.0.16.
-   Google fonts list
-   Added `'flex-height' => true` to `custom-logo` so that cropping is not forced any more.

### New

-   Customizer - Headings & Entry Titles: Added color setting for Widget Titles in the footer sidebar.

### Fix

-	Fixed customizer color control incompatibility with WP version 4.9.
-   Various style.css corrections and optimization.

v1.1.4 - 2017-05-24
--------------------

### New

-   Customizer - Headings & Entry Titles: Added color setting for Widget Titles in left and right sidebar.
-   Customizer - Blog Settings: Hide author name from Post Excerpt and/or Single Post.
-   Customizer - Blog Settings: The comments link now can be textual link or icon. Hide comments link on Post Excerpt and/or Single Post.

### Changed

-   Comments link removed from content.php (and other post parts) and wrapped in `themelia_comments_link()` function.

### Fix

-   Fixed an issue in Customizer which prevented correct color output for Page Title and Entry Title (Single Post).

v1.1.3 - 2017-03-23
--------------------

### Fix

-   Fixed 'Blog Settings' issue that wrongly displayed Full Content by default.

v1.1.2 - 2017-03-23
--------------------

### New

-   Hamburger icon on the mobile menu, now inherits the menu links color
-   Added 'Blog Settings' section in the Customizer. You can switch between displaying Excerpts or Full Content. Applies to the normal post format on the blog page, archives and search results.

v1.1.1 - 2017-03-22
--------------------

### Fixed

-   Style for `btn-primary` and `btn-outline` buttons
-   Reduced top and bottom paddings for better mobile experience
-   An overlap of Hamburger icon and site title and description in Mobile menu

### New

-   Added a few helper classes in style.css

### Updated

-	Format style.css for better readability


v1.1.0 - 2017-03-19
--------------------

### New

-   Added new sidebar named Colophon. Widget added in this sidebar will replace the Copyright line in the site footer.
-   Added new sidebar named Colophon Right, placed in the bottom-right footer of the site.
-   Added `do_action()` functions `themelia_before_content` and `themelia_after_content` for developers to hook into.

### Changed

-	Updated README
-	The description text in README and style.css

v1.0.19 - 2017-03-12
--------------------

### New

-   Added "Footer Left" nav menu location.

### Fixed

-	Fixed style glitches in form elements, buttons and anchors using class `.btn`
-   Removed unused variable `$author_url` from author-box.php

v1.0.18 - 2017-03-10
--------------------

### Fixed

-	Escape `get_theme_mod()` in customize.php
-   Prefix `loop_columns()` function
-   Removed previously dropped `themelia_has_gravatar()` function from author-header.php
-   Removed accidentally added `storefront_make_me_cute()`

### Updated

-	Style tweaks for newsletter widgets. Added style for MailPoet.
-   Update .pot file.

v1.0.17 - 2017-03-04
--------------------

### Changed

-	Removed aria-hidden="true" from post thumbnail
-	Comments link hidden if comments are off
-   Dropped themelia_has_gravatar() function. Display of the author's avatar relies on get_avatar( $author_email ).

### Updated

-	Minor style tweaks for comments-template and author's avatar.
-   Update .pot file.

v1.0.16 - 2017-02-25
--------------------

### Fixed

-	Accessibility issue - The post title in addition to Comments, Read More and Post Edit link was not properly added.
-	Accessibility issue - Color contrast for links hover.

v1.0.15 - 2017-02-21
--------------------

### Fixed

-	Fix Comment link - When there is no post comments do not display link.

v1.0.14 - 2017-02-20
--------------------

### Fixed

-	Accessibility issues - The post title in addition to Comments, Read More and Post Edit link (wrapped in screen-reader-text)

v1.0.13 - 2017-02-20
--------------------

### Fixed

-	Footer widgets on small screens
-	Accessibility issues
-	Footer widgets on small screens
-	Minor style tweaks

v1.0.12 - 2017-01-16
--------------------

### Fixed

-	Search form field bug in IE.
-	Style and Customizer settings for current and hover menu links.
-	Fixed stacked layout for the main menu.
-	Fixed broken footer layout when social menu is not present.
-	Entered correct relationship value for aria-controls attribute in menu/primary.php
-	Other smaller style tweaks

### Changed

-	The footer menu now by default displays textual part of the link so it can be used as a classic menu as well. Inputting a custom link to your social profile the menu item will automatically display an icon for that social network. To hide textual part of the link and display only the icon, add "icon-only" class to each menu item. Find more in the readme file.

v1.0.11 - 2017-01-04
--------------------

### Fixed

-	Enqueuing imagesloaded.js bundled with WordPress core.
-	Pointer/filler content removed from sidebars and widgets.
-	All text strings are translatable - menu/primary.php.

### Changed

-	Theme modification names are changed to be more unified (kirki-conf.php).
-	Changed the way custom style is outputed (change in themelia_customizer_styles() function in inc/customize.php).

### Updated

-	Minor style tweaks.

v1.0.10 - 2016-12-19
--------------------

### New

-	Added support for the JetPack infinite scroll.
-	New screenshot.png

### Changed

-	Opening and closing divs for main container are moved from header.php and footer.php into index.php. Makes it easier creating templates.
-	New screenshot.png

### Updated

-	Lots of cosmetic changes in various files.

v1.0.9 - 2016-12-13
-------------------

### Fixed

-	Added correct version of Ionicons

### Changed

-	Added sanitize.css in place of normalize.css

### Updated

-	SmartMenus jQuery Plugin updated to v1.0.1 which fixes several bugs

v1.0.8 - 2016-12-13
-------------------

### Fixed

-	Style fixes
-	Removed unused scripts

### Updated

-	Ionicons update to version 3.0.0-alpha.3

v1.0.7 - 2016-11-12
-------------------

### Updated

-	Kirki library updated to version 2.3.7

### Changed

-	Added accessibility-ready tag
-	Added SmartMenus jQuery Plugin for the primary desktop and mobile menu
-	Removed Superfish menu
-	Removed SlivkNav menu
-	Removed CodeMirror library from Kirki

v1.0.6 - 2016-09-15
-------------------

### Fixed

-	Fix Windows Phone scale issue in unsemantic.css
-	Fix the issue with media queries and browser zoom using the exact same values for both min-width and max-width in unsemantic.css
-	Fix main nav dropdowns for Stacked-Centered header layout (class .header-s-c)
-	Minor style.css tweak (label margin)
-	Code formatting and cleanup

v1.0.5 - 2016-09-15
-------------------

### Fixed

-	Escaping `get_permalink()` in content/.php files
-	Fix style for showing stacked and centered nav menu
-	CSS tweak for forms (input, textarea width)
-	CSS tweak for Print styles (@media print)

### Changed

-	Removed custom pagination. The function `themelia_paging_nav()` is now a wrapper for the core `the_posts_pagination()` function.
-	Navigation to next/previous post is wrapped in `themelia_post_nav()` function.

### Updated

-	Kirki library updated to version 2.3.6
-	Removed custom panels from Customizer
-	Added theme support for the core Custom Background function

v1.0.4 - 2016-08-29
-------------------

### Fixed

-	Function prefix in customize.php
-	Code cleanup

### Changed

-	Added filters for custom attributes / container id and class - in themelia.php
-	Containers attributes through `hybrid_attr()` function - in header.php
-	Changed CSS media query - mobile menu appears at 1024px

### Removed

-	Unused functions removed from customize.php

v1.0.3 - 2016-08-04
-------------------

### Fixed

-	Function prefix in themelia.php
-	Code cleanup

v1.0.2 - 2016-06-28
-------------------

### Fixed

-	Fixed typos in recent changes in the description text in README and style.css
-	Escaping `home_url()` in searchform.php
-	Escaping urls and code cleanup in author-header.php and author-box.php
-	General code cleanup and other minor improvements

### Changed

-	Added separator in the Author By Line - content/.php
-	File version for enqueued scripts
-	Changed prefix for some functions and filters to suit theme name
-	Changed $handle parameter in the enqueue style.css to suit the theme name
-	Changed $handle parameter in `wp_add_inline_style()`, in accordance with the style.css enqueue
-	Code cleanup and formatting for better readability
-	Removed support for Cleaner Gallery

v1.0.1 - 2016-06-14
-------------------

### Changed

-	Description text in the README and style.css

v1.0.0 - 2016-06-14
-------------------

### New

-	Initial release
