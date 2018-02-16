# Post Format
Camden theme supports [Post Formats](https://codex.wordpress.org/Post_Formats ":target=_blank"), user can change how a post looks by choosing a Post Format.
The theme will display a post differently based on the format chosen.

## Supported Formats

#### Aside
Typically styled without a title. Similar to a Facebook note update.

// tweak styling. remove title

#### Image
A single image. The first `<img />` tag in the post could be considered the image. Alternatively, if the post consists only of a URL, that will be the image URL and the title of the post (post_title) will be the title attribute for the image.

#### Video
A single video or video playlist. The first `<video />` tag or object/embed in the post content could be considered the video. Alternatively, if the post consists only of a URL, that will be the video URL. May also contain the video as an attachment to the post, if video support is enabled on the blog (like via a plugin).

#### Audio
An audio file or playlist. Could be used for Podcasting.

#### Quote
A quotation. Probably will contain a blockquote holding the quote content. Alternatively, the quote may be just the content, with the source/author being the title.

#### Link
A link to another site. Themes may wish to use the first <a href=””> tag in the post content as the external link for that post. An alternative approach could be if the post consists only of a URL, then that will be the URL and the title (post_title) will be the name attached to the anchor for it.

#### Gallery
A gallery of images. Post will likely contain a gallery shortcode and will have image attachments.

// need instruction