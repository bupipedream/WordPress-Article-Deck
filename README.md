#Article Deck
Add a deck to an article published in WordPress.

## Description
This plugin simply adds a meta box named "Article Deck" to the WordPress "Add new post" page. It works by saving a custom field named `_pd_article_deck_text` to the `wp_postmeta` table.

## Usage
Download `article-deck.php` and add it to your theme's `functions.php` file.

Add `<?php echo get_post_meta(get_the_ID(), '_pd_article_deck_text', true); ?>` wherever you wish to display the deck.

## Issues
This script is not perfect by any means. *Please* backup before running this! Here are some possible issues:

- The script continues to run when errors occur.
- Currently only works with MAMP since it assumes that your MySQL CLI is accessible at `/applications/MAMP/library/bin/mysql`. This should be easy  to fix for other systems.

If you encounter other issues, please email [developer@bupipedream](mailto:developer@bupipedream.com).

## Credit
Code based on a [Tuts+ tutorial by Christopher Davis](http://wp.tutsplus.com/tutorials/plugins/how-to-create-custom-wordpress-writemeta-boxes/). Developed by students at [Pipe Dream](http://www.bupipedream.com/), the student-run newspaper at Binghamton University.

**Authors:** 
- Daniel O'Connor / Lead Web Developer
- Christopher Davis (Original Author) / [WordPress Tuts+](http://wp.tutsplus.com)