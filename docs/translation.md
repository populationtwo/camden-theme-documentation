# Translation and RTL Support

This theme is localized, it's ready to be translated and support Right-to-Left languages. The theme come with language files that can be translated to make your site to display on a different language.

These are several translatation management tools to translate this file:

1. [Poedit](https://poedit.net/) — software not a WordPress plugin. Easy and very straightforward, however you'll need to upload the generated language file to the theme folder.
2. [PolyLang](https://wordpress.org/plugins/polylang/) — WordPress plugin, simple.
3. [WPML](https://wpml.org/) — WordPress plugin, it has a lot of features but not suitable for beginner.

These tools can create a new translation from from .POT file (`camden/language`)

## Creating Translation with Poedit
1. Download and install [Poedit](https://poedit.net/).
2. Click **File** > **New from PO/POT file**.
3. Open catalog template file `\wp-content\themes\camden\languages`.
4. Choose the new language.
5. Go through and add/edit your translations by clicking on each string and adding the translation in the bottom box.
6. When you're done, simply click **Save**. Save it in the same directory as the catalog template file.
7. Change the language in the admin settings screen (**Settings** > **General** > **Site Language**).

## RTL (Right-to-Left) Language Support
1. Open `library/enqueue-scripts.php`.
2. Find `wp_style_add_data('main-stylesheet', 'rtl', 'replace')` and uncomment it.
3. Save the file and upload it.
4. Change the language in the admin settings screen (**Settings** > **General** > **Site Language**).
5. The theme will load `camden-style-rtl.css` instead of `camden-style.css`.


**More information about translating WordPress themes**:
- [Installing WordPress in Your Language](http://codex.wordpress.org/WordPress_in_Your_Language)
- [Localization](https://developer.wordpress.org/themes/functionality/localization/)
