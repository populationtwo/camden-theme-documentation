# Translation and RTL Support

This theme is localized, it's ready to be translated and support Right-to-Left languages. The theme come with language files that can be translated to make your site to display on a different language.

These are several translatation management tools to translate this file:

1. [Poedit](https://poedit.net/ ":target=_blank") — software not a WordPress plugin. Easy and very straightforward, however you'll need to upload the generated language file to the theme folder.
2. [PolyLang](https://wordpress.org/plugins/polylang/ ":target=_blank") — WordPress plugin, simple.
3. [WPML](https://wpml.org/ ":target=_blank") — WordPress plugin, it has a lot of features but not suitable for beginner.

These tools can create a new translation from from .POT file (`camden/language`)

## Creating Translation with Poedit
1. Download and install [Poedit](https://poedit.net/ ":target=_blank").
2. Click **File** > **New from PO/POT file**.
3. Open catalog template file `\wp-content\themes\camden\languages`.
4. Choose the new language.
5. Go through and add/edit your translations by clicking on each string and adding the translation in the bottom box.
6. When you're done, simply click **Save**. Save it in the same directory as the catalog template file.
7. Change the language in the admin settings screen (**Settings** > **General** > **Site Language**).

## Creating Translation with Loco Translate
1. Install and activate [Loco Translate](https://wordpress.org/plugins/loco-translate/ ":target=_blank") plugin
2. From your Dashboard go to __Loco Translate__ > __Home__. Click __Camden__ on the __Active theme__ list. 
3. Click the __+ New language__ button on the __Overview__ tab.
4. On the next screen select the desired language and keep the default location (`languages/loco/themes/camden-<locale>.po`).
 Click __Start translating__.
5. On the editor screen you'll see all the strings the theme has defined in its template file. Untranslated strings are shown in bold blue. To start with they will all be untranslated.
6. Select text string from the __Source Text__ list and then Add your translated text in the translation textarea below.
7. Continue to translate as much as you like and when you're ready click the __Save__ icon in the editor toolbar.
8. Congratulations, you've saved your first WordPress translation.

## RTL (Right-to-Left) Language Support
1. Open `library/enqueue-scripts.php`.
2. Find `wp_style_add_data('main-stylesheet', 'rtl', 'replace')` and uncomment it.
3. Save the file and upload it.
4. Change the language in the admin settings screen (**Settings** > **General** > **Site Language**).
5. The theme will load `camden-style-rtl.css` instead of `camden-style.css`.


**More information about translating WordPress themes**:
- [Installing WordPress in Your Language](http://codex.wordpress.org/WordPress_in_Your_Language ":target=_blank")
- [Localization](https://developer.wordpress.org/themes/functionality/localization/ ":target=_blank")
