# Sass 7-1 Boilerplate
**This repository has been updated to more closely reflect the boilerplate written by [Kitty Giraudel](https://github.com/KittyGiraudel/sass-boilerplate). For a more advanced version, use the other repository.**

Base structure with example files:
* abstracts/ (or helpers/ or utils/)
    * _functions.scss
    * _mixins.scss
    * _variables.scss
* base/
    * _color.scss
    * _reset.scss
    * _typography.scss
* components/
    * _buttons.scss
    * _gallery.scss
    * _navigation.scss
* layout/
    * _grid.scss
    * _header.scss
    * _sidebar.scss
* pages/
    * _about.scss
    * _contact.scss
    * _home.scss
* themes/
    * _admin.scss
    * _theme.scss
* vendors/
    * _bootstrap.scss
    * _jquery-ui.scss
* main.scss

The *abstracts, helpers, or utils folder* holds Sass tools, helper files, variables, and config files. These files won’t be compiled. Variables should be project-wide or else placed in their respective component's file.

The *base folder* holds boilerplate content. It contains the styles every page of your site should receive.

The *components folder* holds all your micro layout files. Your styles for buttons and navigation and similar page components.

Your macro layout files go in the *layouts folder*. Styles for major sections of the layout like a header or footer and styles for a grid system would belong here.

If you have styles specific to individual pages on your site, you can place them in the *pages folder*. For example it’s not uncommon for the home page of your site to require page specific styles that no other page receives.

The *themes folder* holds files that create project specific themes. For example one section of your site might use a color scheme with primary colors, while another section builds a color scheme based on neutrals and earth tones.

Finally the *vendors folder* holds 3rd party code and the main.scss file uses @use statements to include the other files.
