# Installation

Installing the theme can be done in two ways. You can upload the theme ZIP file using the built in WordPress theme upload, or copy the files through an FTP client.

0. [**Using WordPress Theme Upload**](#using-theme-upload)
0. [**Uploading by FTP**](#using-ftp)

##### Recommended Additional Steps

We highly recommend the use of child themes. The additional step involves repeating installation steps for **${var.theme-slug}-child.zip** file

?> **Important:** Be sure to extract the file **"${var.theme-slug}.zip"** from the ThemeForest download before uploading. Using the ThemeForest ZIP file directly will result in a "Missing Style Sheet" error.

---

## Using Wordpress Theme Upload :id=using-theme-upload

0. Login to your WordPress admin.
0. In the `Appearance > Themes` menu click the tab **"Install Themes"**
0. At the top of the page click, **"Upload"**, then click the file input to select a file.
0. Select the zipped theme file, **"${var.theme-slug}.zip"** available in **Theme files** folder from the package downloaded from ThemeForest, and click **"Install Now"**
0. After installation you will receive a success message confirming your new install.
0. Click the link **"Activate"**

##### Common Issues

0. **Are You sure you want to do this?** If you get this message. Please check with your webhost upload file size limit and ask them to increase the limitation.
0. **Theme is missing the style.css stylesheet error** This is because you have choosen an invalid theme file. Please follow instruction on [this page](https://help.market.envato.com/hc/en-us/articles/202821510).
0. **Theme install failed destination folder already exists** This is because WordPress allows you to have only 1 theme with the same name and folder. To get around this issue, please update theme using auto updater or FTP steps above.

---

## Uploading by FTP :id=using-ftp

0. Login to your FTP server and navigate to your WordPress themes directory.
0. Normally this would be "**wp-content/themes**"
0. Extract the files from the zipped theme available in the package downloaded from ThemeForest.
0. Copy the folder "**${var.theme-slug}**" to your themes directory.
0. After the files finish uploading, login to your WordPress admin.
0. In the **"Appearance"** menu click **"Themes"**
0. Click **"Activate"** for the theme **"${var.theme-name}"**


---


# Activate the theme

Once the theme is uploaded, activate it from `Appearance > Themes` by clicking the **"Activate"** link for **"${var.theme-name}"**.

After you have activated the theme. You need to install the plugins that are required and recommended to use with the theme.

---

# Plugin Installation

After you had activated the theme, you need to install the plugins required by the theme.

0. After you have activated your theme, you'll see a notice about required plugins for **${var.theme-name}**, to proceed click **"Begin installing plugins"**.
0. On clicking on it, you will be redirected to **Install Required Plugins** Page. Alternatively this page can be accessed from `Appearance > Install Plugins` as well.
0. You will now see a list of plugins required and recommended for use with this theme. Click on the **Select All** checkbox to select plugins.
0. Click on **Bulk Actions** dropdown menu, choose **Install** dropdown option and click the **Apply** button.
0. If all plugins are installed successfully, you will be redirected to WP Plugins page.
0. In case you encounter any problems, try installing theme one by one.
0. After you have installed all the plugins, activate them by navigating to **Plugins** page, select the required plugins, choose activate from the dropdown option and click on **Apply** button.

You have now successfully installed and activated the plugins required for ${var.theme-name} Wordpress Theme.

#### Recommended Plugins

The following is the list of plugins in alphabetical order that are recommended for use with **${var.theme-name}** Wordpress theme.

* **${var.theme-name} Extensions** - This is a custom plugin for enabling extra features such as Review, Shortcodes, Widgets and custom post types. Keeping in mind the plugin territory recommendations by ThemeForest we had implemented custom shortcodes and taxonomies functionalities into a separate plugin.

* **[Gutenberg](https://wordpress.org/plugins/gutenberg/)** — Wordpress Block Editor.

* **[Contact From 7](https://wordpress.org/plugins/contact-form-7/)** — Allows you create contact forms.

* **[Envato Wordpress Toolkit](https://github.com/envato/envato-wordpress-toolkit)** — This toolkit plugin establishes an Envato Marketplace API connection to take advantage of the new `wp-list-themes` & `wp-download` methods created specifically for this plugin.

* **[Regenerate Thumbnails](https://wordpress.org/plugins/regenerate-thumbnails/)** - Allows you to regenerate your thumbnails after changing the thumbnail sizes.

* **[Slider Revolution](http://codecanyon.net/item/slider-revolution-responsive-wordpress-plugin/2751380/?ref=envirra)** - Allows you to create a responsive(mobile friendly) or fullwidth slider with must-see-effects and meanwhile keep or build your SEO optimization. This is a premium plugin and comes bundled with your theme.

* **[WooCommerce](https://wordpress.org/plugins/woocommerce/)** — WooCommerce is a powerful, extendable eCommerce plugin that helps you sell anything. Beautifully.

---

# Import Demo Content

Before importing demo content, Please make sure the **${var.theme-name}** theme and **Envirra Extensions** plugin is already activated.

0. Install plugin for importing demo content by go to menu `Appearance > Install Plugins` and click **Install** and **Activate** of the plugin **One Click Demo Import**.
0. Go to menu `Appearance > Import Demo Data`.
0. Click **Import** button of the demo you want to import. All demo content will be downloaded. Please note that some site configuration may be overridden by demo's configuration. **Do not interrupt it**.
0. If you see some messages about **invalid post type**, It's ok to ignore that.
0. If you see some messages about failed to import media, It's ok to ignore that. But if you need all demo images to be shown on your site, Please import again.
0. Some blocks and widgets may have a difference from the demo site due to a limitation of importing.

?> **Important:** Please do not import content on a WordPress installation that already has a lot of content. Or the very least, make a backup first. A catastrophic mess can be created.

---

# How to update the theme	

You can update your theme via FTP or via WordPress. See the information below for each method. No matter what method you choose, you first need to download the new theme files from Themeforest.

#### Prerequisites for updating the theme

0. First you need to download the latest version of theme. Log into your Themeforest account and navigate to your downloads tab. Find the **${var.theme-name}** theme purchase.
0. Click the **download** button next to it and choose to download the **Installable WordPress Theme** which is just the WordPress file, or choose the **Main Files** which is the entire package which include theme documentation, plugins etc.
0. Backup your site before updating the theme. Please follow the steps via using a plugin to automatically backup your current theme and uploading the new version: http://wordpress.org/extend/plugins/easy-theme-and-plugin-upgrades/
0. Backup Setting of Customizer before updating the theme. Please use plugin [Customizer Export/Import](https://wordpress.org/plugins/customizer-export-import/) to backup the setting of Customizer.

#### Method 1 : Update using Envato Market Plugin

0. You need to download the plugin from here.
0. Go to `Themeforest > You Account > Settings > API Key` and copy API Key.
0. Click the **Envato Market** menu in WordPress Dashboard.
0. Enter your API Key and you will be able to see your purchased items which is included ${var.theme-name} theme

#### Method 2 : Update using plugin

0. You need to download and install Easy Theme and Plugin Update.
0. After installing the plugin. Go to `Apperance > Themes > Add New > Upload Theme`
0. Select the downloaded ZIP file and choose **Upgrade existing theme** option to **Yes** and click **Install Now** button

#### Method 3 : Update using WordPress Dashboard

0. You may want to use a plugin to automate backing up your current theme and uploading the new version: http://wordpress.org/extend/plugins/easy-theme-and-plugin-upgrades/
0. You need to deactivate **${var.theme-name}** theme in the `Appearance > Themes` by simply activating a different theme. Once you activate a different theme, you can delete the ${var.theme-name} theme. Don’t worry. You really won’t loose any of your data.
0. Get the installable zip file from `Themeforest > Account > Download`. If you downloaded the **Main Files** from Themeforest, then you need to unzip the archive file you received, the **${var.theme-slug}.zip** will be inside of it.
0. Upload the zip file using `Appearance > Themes`. Once you uploaded successfully, activate the theme.

#### Method 4 : Update using FTP

0. You may want to use a plugin to automate backing up your current theme and uploading the new version: http://wordpress.org/extend/plugins/easy-theme-and-plugin-upgrades/
0. Login to your FTP account. Navigate to `wp-content/themes` location and backup your **${var.theme-slug}** theme folder by saving it to your computer, or you can choose to simply delete it. Don’t worry. You really won’t loose any of your data.
0. Get the installable zip file from `Themeforest > Account > Download`. If you downloaded the **Main Files** from Themeforest, then you need to unzip the archive file you received, the **${var.theme-slug}.zip** will be inside of it.
0. Drag and drop the new **${var.theme-slug}** theme folder into `wp-content/themes` and select **Replace** if you didn’t delete it.

#### Method 5 : Updating from existing theme

If you update your existing blog site to ${var.theme-name} theme. You have to run [this plugin](https://wordpress.org/plugins/regenerate-thumbnails/) to regenerate all posts's thumbnails from your existing theme setting. Once you installed the plugin, open `Tools > Regen. Thumbnails` and click on **Regenerate Thumbnails** button.

#### Common Issues

0. **Are You sure you want to do this?** If you get this message. Please check with your webhost upload file size limit and ask them to increase the limitation.
0. **Theme is missing the style.css stylesheet error** This is because you have choosen an invalid theme file. Please follow instruction on [this page](https://help.market.envato.com/hc/en-us/articles/202821510).
0. **Theme install failed destination folder already exists** This is because WordPress allows you to have only 1 theme with the same name and folder. To get around this issue, please update theme using auto updater or FTP steps above.