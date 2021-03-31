# Translation

Theme includes bunch of PO translation files for each languages so you can use standard translation tools to help translate theme output strings to your desired language.

### WordPress Language Setting

For WordPress 4.0 + users please follow below steps

1. Login to your WordPress Dashboard and navigate to `Settings > General Settings`
2. Make sure **Site Language** option is set to your desired language.

### Storing Translation Files

Theme use PO translation file which is industry standard translation method. In theme folder you will find a folder called languages. You will find each languages files store in the folder. By default storing inside theme folder. The theme language folder is `wp-content/themes/${var.theme-slug}/languages` or `wp-content/themes/${var.theme-slug}-child/languages/` if you
re using child theme.

`*.POT` – A template file for translation

`*.PO` – A lists of all text strings in theme. The text strings are in English and you can add translation to each of text string.

`*.MO` – This is the compiled .po file and is used by WordPress to translate the theme

If your language isn’t included in the theme language files. You have to create a new .PO file from original `${var.theme-slug}.po` located in theme’s languages folder then save the new .PO file with your language code for example `de_DE.po`

This method has one downside. Because whenevery you update the theme. The whole language folder will be replaced with original version which overwrite your translation files. So the solution is to backup your translation file before updating theme.

---

## Using Poedit Application

Poedit application is the popular application uses to edit .PO file translation and it’s free. [Click here to download Poedit application](https://poedit.net).

Now download and install Poedit application. Open language file you want to translate for example `en_US.po` You will find all English string in Source Text box. Select text string you want to translate, add your translation text to **Translation** field. Once you finish translating. Save the file and it will automatically compiled to `.mo` file.

1. Open file `wp-content/themes/${var.theme-slug}/languages/${var.theme-slug}.pot` using [POEdit](http://www.poedit.net/)
2. Click **Create new translation** button and choose the language.
3. Translate the text.
4. Hit save, a new .PO and .MO file will be created.
5. In case you're using child theme, Please place the .PO and .MO file in child theme folder `wp-content/themes/${var.theme-slug}-child/languages/`.
6. Dont't forget to backup the created .PO and .MO files.

---

## Rename/Change Words

1. Open file `wp-content/themes/${var.theme-slug}/languages/${var.theme-slug}.pot` using [POEdit](http://www.poedit.net/)
2. Click **Create new translation** button and choose the **English** language.
3. Change the words you want.
4. Hit save, a new .PO and .MO file will be created.
5. In case you're using child theme, Please place the .PO and .MO file in child theme folder `wp-content/themes/${var.theme-slug}-child/languages/`.
6. Dont't forget to backup the created .PO and .MO files.

---

## RTL Support

For languages that read from right-to-left unlike English which is left-to-right, ${var.theme-name} theme will automatically switch to an RTL style, as long as you it's in your language and uses the correct locale (as explained above).