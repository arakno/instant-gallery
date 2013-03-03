============================================
Instant Gallery - a simple dynamic gallery to showcase your projects
Version 0.4

Installation and usage instructions
Paulo Basto 2013
www.arakno.net
============================================

------------
Documentation
------------

   1. Installation
   2. Configuration



1. Installation

1.1 Unpack the files, and copy them to your server, for example to /home/youruser/public_html/instant-gallery/

1.2 The folder "portfolio" is where you should create your directories and throw your images in it. The PHP

script will take care of creating a navigation tab for each folder from the folder name, so keep that in mind

when naming your folders.

../instant-gallery/portfolio
        - /catg x
        - /catg y
        - /catg z


2. Configuration

2.1. Image thumbnails are generated into the "cache" folder(duh!). You can configure the thumbnails proportions

in index.php

define( 'THUMBNAIL_IMAGE_MAX_WIDTH', 160 );
define( 'THUMBNAIL_IMAGE_MAX_HEIGHT', 104 );

2.2 Unless stated otherwise 'portfolio/default' is the default folder for your projects. You can alter this

behaviour by modifying the $catg variable of index.php to a folder of your choice.


------------
Changes from version 0.4
------------

++ added quickconcat to streamline http requests
++ improved CSS3 animations and design
++ added drag'n'drop functionality to photos so you can play around
++ responsive layout
-- removed buggy drag'n'drop upload functionality. I am working on a better solution