=== 3D Wall FX ===
Contributors: flashxml
Tags: images, photos, widget, post, plugin, posts, sidebar, free, flash, as3, wall, 3d, gallery, thumb, thumbs, zoom, columns, rows, effect, tootip, flat, xml, rotate
Requires at least: 2.8.0
Tested up to: 2.9.2
Stable tag: trunk

== Description ==

One of the most advanced 3D Wall on the web. Completely XML customizable, without using Flash. And it's free!

= Main features =

You can integrate it in any website for free without even using Flash. Customizable width and height of the overall wall, up to 1680 x 1050 pixels. You can customize the number of columns and lines, items spacing, speed, radius and also the perspective and camera distance from wall. You can have different types of wall: flat, outside 

== Installation ==

Make sure your Wordpress version is equal or greater than 2.8 and your hosting provider is using PHP5.

1. Upload the `3d-wall-fx` directory along with all its files to the `/wp-content/plugins/` directory
2. Activate the plugin through the 'Plugins' menu in WordPress
3. In the post editor use the following tag to embed the 3D Wall: `[3d-wall-fx][/3d-wall-fx]`. Or add `<?php wallfx_echo_embed_code(); ?>` in your templates
4. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your 3D Wall](http://www.flashxml.net/3d-wall.html "3D Wall") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `3d-wall-fx/component/settings.xml`
5. To use your own images, upload them to the `3d-wall-fx/component/images` directory and update the `3d-wall-fx/component/images.xml` file accordingly

= Additional settings file =

To embed the 3D Wall more than once, you will need another settings file and (probably) another set of images. Let's assume your new file is called **settings2.xml**. From the post editor, use the following code: `[3d-wall-fx settings="settings2.xml"][/3d-wall-fx]`. From the PHP files of your theme, add the file name as *the first argument* of the `wallfx_echo_embed_code()` function call. If you use a separate set of images, don't forget to create a new XML file for that and update the `imagesXML` value in the settings file.

= No Flash support text =

To support visitors without Adobe Flash, you can provide alternative textual content. From the post editor, add the text between `[3d-wall-fx]` and `[/3d-wall-fx]`. From the PHP files of your theme, add the text as *the second argument* of the `wallfx_echo_embed_code()` function call.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/3d-wall.html "3D Wall") is the utility that helps easily customize your 3D Wall to fit all of your needs.