=== Relocate Upload ===
Contributors: alanft,tberneman
Tags: admin, upload, folder, relocate, move
Requires at least: 2.8
Tested up to: 5.3.2
Stable tag: 0.24

Wordpress uploads media to one pre-set folder. Relocate Upload lets you switch media to other folders.

== Description ==
Relocate Upload lets you specify folders, and adds a menu to the Media Library (and Edit Media admin page) that lets you switch media items between these folders and WPs default upload location.

== Installation ==
1. Upload the whole 'relocate-upload' folder to the plugins directory.
2. Activate the plugin through the 'Plugins' menu in WordPress.
3. Specify your folders in the settings page.

== Frequently Asked Questions ==
= Why? What's the point of these other folders? =
Most servers are set up so that assets can only be used when referred from your own site - to stop bandwidth leeching. However folders can be set aside that don't obey this rule - e.g. for placing images on other sites, downloading mp3s from RSS feeds and so on.

== Known Issues ==
When creating new folders, 

== Screenshots ==
1. A simple menu switches media assets to your favourite locations. All through the magic of AJAX.
2. A simple settings page to define the folder locations.

== Changelog ==
0.24.1 - Tested compatibility up to WordPress Version 4.7
         Added code changes thanks to Ciprian Tepes which included fixing a path issue and making it work with multisite.

0.24 - Tested compatibility up to WordPress Version 4.2.4
       Fixed several path issues.
	   Added generic "FAIL" message instead of not reporting anything.
       Create folder using WordPress "wp_mkdir_p" function and should set permissions too.
	   
0.23 - Added drag-n-drop to reorder folders.
       Changed root folder variable to WP constant ABSPATH.
	    * This MAY affect your folder locations - BE SURE TO CHECK THEM!
       Formatted source code to be inline with WordPress standards
		
0.22 - Plugin officially taken over by Tim Berneman (tberneman).
       Fixed problem where "remove location" button was not showing up.
	    * Created "images" folder and put "xit.gif" in it.
	    * Does NOT delete the folder or any files in it.
	   Folder is created if it doesn't exist when adding new location.

0.21 - Fixed problem where folder dropdown was not showing in Media edit screen on newer versions of WordPress.

0.20 - Adopted proper 'wp_ajax_' action, to close off a major security issue.

0.14 - Many small fixes (check for existing files, database prefix bug fix, jquery enqueue, 2.8 media library update, path 'fixing').

0.11 - First tiny bug fix (no thumbnails caused an error).

0.10 - Just starting out, something to get it working.