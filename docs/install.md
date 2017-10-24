# Installation & Update

Camden theme can only be used with a working version of WordPress. We strongly recommend you to do a fresh WordPress installation and integrate your content into the pages accordingly. This theme has specific settings that might conflict with your current WordPress themes, plugins, database, etc.

?>This page contain beginners guide to WordPress theme, skip to [the next page]() if you are already comfortable with WordPress.

If you need help installing WordPress, follow the documentation in WordPress Codex . Below are some useful WordPress information to help you get started:

- [WP101 Basix Training videos](https://code.tutsplus.com/series/beginning-with-wordpress--wp-33808) — some great videos from TutsPlus on WordPress
- [WordPress Lessons](http://codex.wordpress.org/WordPress_Lessons) — general information that covers a vast array of topics
- [FAQ New To WordPress](http://codex.wordpress.org/FAQ_New_To_WordPress) — the most popular FAQ’s regarding WordPress

## WordPress Installation

1. Download and unzip the WordPress package if you haven't already.
2. Create a database for WordPress on your web server, as well as a MySQL user who has all privileges for accessing and modifying it.
3. (Optional) Find and rename wp-config-sample.php to wp-config.php , then edit the file (see Editing wp-config.php ) and add your database information.
4. Upload the WordPress files to the desired location on your web server:
   - If you want to integrate WordPress into the root of your domain (e.g. http://example.com/ ), move or upload all contents of the unzipped WordPress directory (excluding the WordPress directory itself) into the root directory of your web server.
   - If you want to have your WordPress installation in its own subdirectory on your web site (e.g. http://example.com/blog/ ), create the blog directory on your server and upload the contents of the unzipped WordPress package to the directory via FTP.
   - Note: If your FTP client has an option to convert file names to lower case, make sure it's disabled.
5. Run the WordPress installation script by accessing the URL in a web browser. This should be the URL where you uploaded the WordPress files.
   - If you installed WordPress in the root directory, you should visit: http://example.com/
   - If you installed WordPress in its own subdirectory called blog , for example, you should visit: http://example.com/blog/

More detailed instructions follow.

It is recommended to install `docsify-cli` globally, which helps initializing and previewing the website locally.

```bash
npm i docsify-cli -g
```

## Initialize

If you want to write the documentation in the `./docs` subdirectory, you can use the `init` command.

```bash
docsify init ./docs
```

## Writing content

After the `init` is complete, you can see the file list in the `./docs` subdirectory.

* `index.html` as the entry file
* `README.md` as the home page
* `.nojekyll` prevents GitHub Pages from ignoring files that begin with an underscore

You can easily update the documentation in `./docs/README.md`, of course you can add [more pages](more-pages.md).

## Preview your site

Run the local server with `docsify serve`. You can preview your site in your browser on `http://localhost:3000`.

```bash
docsify serve docs
```

?> For more use cases of `docsify-cli`, head over to the [docsify-cli documentation](https://github.com/QingWei-Li/docsify-cli).

## Manual initialization

If you don't like `npm` or have trouble installing the tool, you can manually create `index.html`:

```html
<!-- index.html -->

<!DOCTYPE html>
<html>
<head>
  <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1">
  <meta charset="UTF-8">
  <link rel="stylesheet" href="//unpkg.com/docsify/themes/vue.css">
</head>
<body>
  <div id="app"></div>
</body>
<script src="//unpkg.com/docsify/lib/docsify.min.js"></script>
</html>
```

If you installed python on your system, you can easily use it to run a static server to preview your site.

```bash
cd docs && python -m SimpleHTTPServer 3000
```

## Loading dialog

If you want, you can show a loading dialog before docsify starts to render your documentation:

```html
  <!-- index.html -->

  <div id="app">Please wait...</div>
```

You should set the `data-app` attribute if you changed `el`:

```html
  <!-- index.html -->

  <div data-app id="main">Please wait...</div>

  <script>
    window.$docsify = {
      el: '#main'
    }
  </script>
```

Compare [el configuration](configuration.md#el).