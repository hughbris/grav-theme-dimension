# Dimension Theme

The **Dimension** Theme is for [Grav CMS](http://github.com/getgrav/grav). It's a port of [Dimension](https://html5up.net/dimension) by HTML5 UP under its [Creative Commons Attribution 3.0 Unported license](http://creativecommons.org/licenses/by/3.0/).

![Dimension](screenshot.jpg)

# Installation

Installing the Dimension theme can be done in one of two ways. Our GPM (Grav Package Manager) installation method enables you to quickly and easily install the theme with a simple terminal command, while the manual method enables you to do so via a zip file.

## GPM Installation (Preferred)

The simplest way to install this theme is via the [Grav Package Manager (GPM)](http://learn.getgrav.org/advanced/grav-gpm) through your system's Terminal (also called the command line).  From the root of your Grav install type:

    bin/gpm install dimension

This will install the Dimension theme into your `/user/themes` directory within Grav. Its files can be found under `/your/site/grav/user/themes/dimension`.

>> This method will copy the sample pages provided in the `_demo/pages` folder to your `user/pages` folder so that the theme will work out of the box with placeholder content. The content is the same _Ipsum lorem_ content provided in the original [HTML5 UP theme](https://html5up.net/dimension).

## Manual Installation

To install this theme, just download the zip version of this repository and unzip it under `/your/site/grav/user/themes`. Then, rename the folder to `dimension`. You can find these files either on [GitHub](https://github.com/hughbris/grav-theme-dimension) or via [GetGrav.org](http://getgrav.org/downloads/themes).

You should now have all the theme files under

    /your/site/grav/user/themes/dimension

>> NOTE: If you want to use and adapt the default _Ipsum lorem_ content provided with the original theme, move the contents of `_demo/pages` into your grav installations's `user/pages` directory. This will ensure that the theme templates work out of the box.

# Updating

As development for the Dimension theme continues, new versions may become available that add additional features and functionality, improve compatibility with newer Grav releases, and generally provide a better user experience. Updating Dimension is easy, and can be done through Grav's GPM system, as well as manually.

## GPM Update (Preferred)

The simplest way to update this theme is via the [Grav Package Manager (GPM)](http://learn.getgrav.org/advanced/grav-gpm). You can do this with this by navigating to the root directory of your Grav install using your system's Terminal (also called command line) and typing the following:

    bin/gpm update dimension

This command will check your Grav install to see if your Dimension theme is due for an update. If a newer release is found, you will be asked whether or not you wish to update. To continue, type `y` and hit enter. The theme will automatically update and clear Grav's cache.

## Manual Update

Manually updating Dimension is pretty simple. Here is what you will need to do to get this done:

* Delete the `your/site/user/themes/dimension` directory.
* Download the new version of the Dimension theme from either [GitHub](https://github.com/hughbris/grav-plugin-dimension) or [GetGrav.org](http://getgrav.org/downloads/themes#extras).
* Unzip the zip file in `your/site/user/dimension` and rename the resulting folder to `dimension`.
* Clear the Grav cache. The simplest way to do this is by going to the root Grav directory in terminal and typing `bin/grav clear-cache`.

> Note: Any changes you have made to any of the files listed under this directory will also be removed and replaced by the new set. Any files located elsewhere (for example a YAML settings file placed in `user/config/themes`) will remain intact.

# Setup

If you want to set Dimension as the default theme, you can do so by following these steps:

* Navigate to `/your/site/grav/user/config`.
* Open the **system.yaml** file.
* Change the `theme:` setting to `theme: dimension`.
* Save your changes.
* Clear the Grav cache. The simplest way to do this is by going to the root Grav directory in Terminal and typing `bin/grav clear-cache`.

Once this is done, you should be able to see the new theme on the frontend. Keep in mind any customizations made to the previous theme will not be reflected as all of the theme and templating information is now being pulled from the **dimension** folder.

# Usage

## Configuration

Default configuration:

```yaml
icon: gem
# hero_image:
# credit_blurb: 
```
## Supported Page Templates

* [Home template](templates/home.html.twig)
* [Simple homepage modal dialog module template](templates/modular/dialog.html.twig)
