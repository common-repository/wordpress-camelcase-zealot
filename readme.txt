=== Plugin Name ===
Contributors: neil_pie
Donate link: http://www.justgiving.com/stlukesbd/
Tags: camel case, wordpress, autocorrect, capital P
Requires at least: 2.3.0
Tested up to: 4.4
Stable tag: 0.2.4
License: WTFPL
Blindly enforces the correct CamelCasing of 'WordPress' throughout frontend of site.

== Description ==

Having 'Wordpress' automatically switched to 'WordPress' in just a few spots around your site not enough for you? Want the rules to be applied with a little more zeal? This plugin tries to enforce the correct CamelCasing of 'WordPress' throughout your site irrespective of whether or not it begins with a capital letter 'W'. 

Currently:

* Post Content 
* Post Title
* Page Lists
* Category Lists
* Tag Lists
* Nav Menus
* Bloginfo
* Comments
* Tag Cloud
* Widget Titles
* Text Widget Content
* Manual & Automatic Post Excerpts

Be warned, at the moment this plugin will also make the changes in link and image URLs, which may cause them to break on some server setups.

== Installation ==

1. Upload `wordpress-camelcase-zealot.php` to the `/wp-content/plugins/` directory
1. Activate the plugin through the 'Plugins' menu in WordPress
1. Sleep soundly at night, safe in the knowledge that there a few more capital 'P's on the internet 

== Frequently Asked Questions ==

= Will this plugin break my links and images? =

It might do. On some server setups, http://hello.com/wordpress.jpg is a different file to http://hello.com/WordPress.jpg - be sure you test this out before using the plugin.

= Why doesn't it catch everything? =

In all honesty, because it's a work in progress. Rather than fill in every filter possible, I'm trying to add them as I come across them. Let me know where I've missed it on your site & I'll add it next release.

= Does it have to be so thorough? =

No. If you hook onto the `wpccz_added_filters` filter hook you will have access to the array of filter hooks to which we are applying the string replace. Remove any that you don't wish to use. Similarly, you can add any that are missing.

== Screenshots ==

1. just look at all those capital Ps

== Changelog ==
= 0.2.4 =
Added wpccz_added_filters filter hook
= 0.2.3 =
Housekeeping
= 0.2.2 =
Housekeeping
= 0.2.1 =
Prevented the plugin from messing around with editor fields in wp-admin by only running it on the front-end. You rdata is safe again. Added a few more filter hooks.
= 0.1.1 =
Changed the readme file to meet the WordPress guidelines.
= 0.1 =
First commit

== Upgrade Notice ==
= 0.2.4 =
A new filter hook has been added in this release. View readme for details.
= 0.2.3 =
Housekeeping - no need to update
= 0.2.2 =
Housekeeping - no need to update
= 0.2.1 =
Added more filter hooks & isolated plugin to front end - no more DB writing!
= 0.1.1 = 
No code changes. Upgrade not require
= 0.1 =
First Version
