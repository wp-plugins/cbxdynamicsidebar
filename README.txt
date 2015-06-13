=== CBX Dynamic Sidebar ===
Contributors: manchumahara,codeboxr,wpboxr
Donate link: http://wpboxr.com/donate
Tags: sidebar, widgets, dynamic
Requires at least: 3.0.1
Tested up to: 4.2.2
Stable tag: 1.0.1
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Dynamic sidebar for wordpress using custom post type and shortcode

== Description ==

CBX Dynamic Sidebar for Wordpress helps to create dynamic sidebar or widget position using custom post type. Sometimes we need to put sidebar inside content and this plugin
 helps to create sidebar using custom post type and put the sidebar inside content using shortcode using simple shortcode

 [cbxdynamicsidebar id="post id here" /] 

 It'a also possible to call the sidebar using direction function call in theme

 `<?php
   if(function_exists('cbxdynamicsidebar_display')){
     $sidebar_id   = 'post id here';
  	 $config_array = array(
  		 'id'            => $sidebar_id,
  		 'wclass'        => 'cbxdynamicsidebar_wrapper',
  		 'wid'           => 'cbxdynamicsidebar_wrapper',
  		 'float'         => 'auto'
  	 );
  	 echo cbxdynamicsidebar_display($config_array);
   }

  ?>`

  or more simple way

  <?php
    do_shortcode('[cbxdynamicsidebar id="post id here"]');
   ?>

   See the gist here https://gist.github.com/manchumahara/81c60c90d03678a1964c#file-gistfile1-txt

From the custom post type "cbxsidebar" post edit screen there are other features that is implemented using meta field for

- sidebar class
- sidebar description
- sidebar before widget html wrapper
- sidebar after widget html wrapper
- sidebar widget before title html wrapper
- sidebar widget after title html wrapper
- sidebar enable disable without deleting the sidebar post
- Translation ready


Shortcode & function Param Definition
id – sidebar post id

wclass – sidebar will be wrapper in a div and it will have a class from the value of param ‘wclass’, default value is ‘cbxdynamicsidebar_wrapper’. also extra another class will be added using ‘cbxdynamicsidebar_wrapper’ with sidebar id at last

wid – sidebar will be wrapper in a div and it will have a class from the value of param ‘cbxdynamicsidebar_wrapper’, default value is ‘cbxdynamicsidebar_wrapper’ with sidebar id at last

float – default value ‘auto’, other possible values ‘left’, ‘right’, which means float none/auto, float left and float right

For shortcode with all possible param –

[cbxdynamicsidebar id="post id here" float="left" wclass="cbxdynamicsidebar_wrapper" wid="cbxdynamicsidebar_wrapper" /]

For more details check here http://wpboxr.com/product/cbx-dynamic-sidebar-for-wordpress

== Installation ==

This section describes how to install the plugin and get it working.

e.g.

1. Upload `cbxdynamicsidebar` folder to the `/wp-content/plugins/` directory
2. Activate the plugin through the 'Plugins' menu in WordPress

== Frequently Asked Questions ==



== Screenshots ==

1. Sidebar Listing with shortcode note
2. Single Sidebar Edit
3. Widget assign in sidebar from admin panel
4. Frontend Dynamic sidebar appears from shortcode

== Changelog ==

= 1.0.1 =
* First Release

== Upgrade Notice ==

= 1.0 =
Upgrade notices will be here if available
