# Site Custom

Starter kit for site-specific custom modules, including a few small, commonly useful bits of code

## To use

1. Rename site_custom.info and site_custom.module files to XXX_custom.info, where XXX is a machine-safe version of your site name (all lowercase alphanumeric characters and underscores)
2. Do a global search-and-replace in both files to replace the string "site_custom" with "XXX_custom" (XXX as above)
3. Do a global search-and-replace in both files to replace the string "site_name" with your site's name
4. Add any custom code for your site to the .module file, using XXX_custom as the hook name. Administrative options can be added to the form defined in the _XXX_custom_config() function

## Includes

1. option to display /styles page which displays common HTML elements and Drupal form elements on a single page, to aid in theme development
2. an option to make an arbitrary link in a menu turn into a language-switcher for bilingual sites, per [this tutorial](http://www.liquidcms.ca/post/how-language-switcher-menu-item) __Note:__ this only works on menus that are rendered through the regular Drupal theming engine, and will not work with the main menu on the [webskillet base theme](https://github.com/webskillet/webskillet), which uses menu_tree to render the menu, or modules like [OM Maximenu](https://www.drupal.org/project/om_maximenu).