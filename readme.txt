=== 3D Wall FX ===
Contributors: flashxml
Tags: images, photos, widget, post, plugin, posts, sidebar, free, flash, as3, wall, 3d, gallery, thumb, thumbs, zoom, columns, rows, effect, tootip, flat, xml, rotate
Requires at least: 2.8.0
Tested up to: 3.0
Stable tag: trunk

== Description ==

One of the most advanced 3D Wall on the web. Completely XML customizable, without using Flash. And it's free!

= Main features =

You can integrate it in any website for free without even using Flash. Customizable width and height of the overall wall, up to 1680 x 1050 pixels. You can customize the number of columns and lines, items spacing, speed, radius and also the perspective and camera distance from wall. You can have different types of wall: flat, outside and inside curvature with different types of movement and tweening functions. The thumbs have glow and blur effects, you can link to an URL on clicking a thumb instead of enlarging it, the tooltips have a lot of properties and the scroll bar can be skinnable.

== Installation ==

Make sure your Wordpress version is greater than 2.8 and your hosting provider is using PHP5.

1. [Download](http://www.flashxml.net/free/download/3d-wall.zip "3D Wall FX") or [purchase](http://www.flashxml.net/3d-wall.html#swmi-license "3D Wall FX") the 3D Wall FX Flash component
2. Create a new folder inside your `/wp-content/` directory called `flashxml/3d-wall-fx` and copy the content of the archive to this folder
3. Install [the plugin](http://downloads.wordpress.org/plugin/3d-wall-fx.zip "3D Wall FX Plugin") or upload the `3d-wall-fx` folder along with all its files to `/wp-content/plugins/` directory
4. Activate the plugin from the **Plugins** tab in **WordPress Dashboard**
5. Go to **3D Wall FX** from the **Settings** tab and update the path in case you used a different one
6. In the post editor use the following tag to embed the 3D Wall FX: `[3d-wall-fx][/3d-wall-fx]`. You could also add `<?php wallfx_echo_embed_code(); ?>` in the PHP file of your theme
7. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your 3D Wall FX](http://www.flashxml.net/3d-wall.html "3D Wall FX") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `flashxml/wallfx/settings.xml`
8. To use your own images, upload them to the `flashxml/wallfx/images` folder and update the `flashxml/wallfx/images.xml` file accordingly

= Additional settings file =

To embed the 3D Wall FX more than once, you will need another settings file and (probably) another set of images. Let's assume your new file is called **settings2.xml**. From the post editor, use the following code: `[3d-wall-fx settings="settings2.xml"][/3d-wall-fx]`. From the PHP files of your theme, add the file name as *the first argument* of the `wallfx_echo_embed_code()` function call. If you use a separate set of images, don't forget to create a new XML file for that and update the value in the settings file.

= No Flash support text =

To support visitors without Adobe Flash, you can provide alternative textual content. From the post editor, add the text between `[3d-wall-fx]` and `[/3d-wall-fx]`. From the PHP files of your theme, add the text as *the second argument* of the `wallfx_echo_embed_code()` function call.

= If you have PHP4 =

To make it work if you're using PHP4, add the following code `[3d-wall-fx width="600" height="300"][/3d-wall-fx]` in the post editor. From the PHP files of your theme, add the width and height as *the third and fourth argument* of the `wallfx_echo_embed_code()` function call. Don't forget to provide your own width and height values, since 600 and 300 are just examples.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/3d-wall.html "3D Wall FX") is the utility that helps easily customize your 3D Wall FX to fit all your needs.