# Basic Setup

## Setting Up Home Page

1. Navigate to **Pages** > **Add New**.
2. Select **Home Page Template** as the template from the **Page Attributes**.
3. Add a title and content you would like to see within the content area of the static front page, or leave it blank.
4. Publish the Page.
5. Navigate to **Settings** > **Reading**.
6. Select **A static page** option for the **Front page displays**.
7. Select the page you just created as the **Front page**.
8. Navigate to **Theme Options** > **Front Page** and [configure the settings]().

![Reading Setting Front Page](_images/reading-setting-front-page.png)

## Setting Up Blog page

1. Navigate to **Pages** > **Add New**.
2. Select **Default Template** as the template from the **Page Attributes**.
3. Add a title and Publish the Page.
4. Navigate to **Settings** > **Reading**
5. Select **A static page** option for the **Front page displays**.
6. Select the page you just created as the **Posts page**.

![Reading Setting Post Page](_images/reading-setting-posts-page.png)

## Page Templates
A Page Template is a template which comes with your theme. WordPress can be configured to use different Page Templates for different Pages. Page templates are used to change the look and feel of a page. You can select which Template will be used when displaying a particular Page.

Camden theme comes with unique page templates which adds additional functionality to your pages. These are the page templates that can be found in this theme:

1. **Home Page** — a page template for Front Page
2. **Full Width Page** — a full width page template without the sidebar.
3. **Times & Directions Page** — a page template to display map and service times.
4. **Contact Page** — a page template with contact form

### How To Change a Page Template

1. Navigate to **Pages** and select the page
2. On the right hand side under **Page Attributes** you’ll see template. This is where users are able to access your global page templates.
3. Select the Page Template.

![Page Template Dropdown](_images/page-template-dropdown.png)

?>**Could not find the Page Attribute panel?**  
  If you do not see this panel, look to the top right of your screen for **Screen Options**. Click **Screen Options** and check the **Page Attributes** checkbox.
  
### Contact Page
Camden theme comes with a Contact Page template to embed contact form in a single column. You will need contact form plugin such as Contact Form 7 or Gravity Form. We recommend Contact Form 7, since Camden theme integrate custom styling for Contact Form 7 elements.

#### Setting up Contact Page
1. Make sure contact form plugin is activated. We use Contact Form 7 for this example.
2. Create a new Page and change the Template to Contact Page.
3. Create your custom contact form. Check the Contact Form 7 guide for more details.
4. Copy the Contact Form 7 embed code and add it to the contact page text editor.
![Contact Page Embed Code](_images/contact-page-contact-embed-code.png) 
5. Fill the Contact Info fields with additional info such as address and phone number. 
![Contact Page Contact Info](_images/contact-page-contact-info.png)

### Times & Direction Page
Camden theme comes with a Times & Direction template to display service times and map. Change page template to **Times & Direction** to enable it.

#### Times & Direction Options

**Service Times Entry**  
Define the service times. It accepts HTML and multiple entries. 

Recommended markup:
```html
<dl>
    <dt>TITLE</dt>
    <dd><span class="time">12:00 AM</span>
    LOCATION
    <a href="URL">View Details</a></dd>
</dl>
```

**Map Image**  
Define the map image URL. You can upload the map image to WordPress Media Library ( Media > Library ) and get the image URL. Alternatively, you may use map image maker such as [Static Map Maker](http://staticmapmaker.com/) to generate the URL.
       
**Direction Info**  
Add short additional info to be displayed next to the map image. It accepts HTML.

**Map URL**  
Define the URL where the Map Image links to, usually it's the share link. 

```html
//Google Map
https://www.google.com/maps/@18.5411754,-80.1912377,15z

//Bing Map
https://binged.it/2fAzbZF
```

## Page Options

Page Options is available on all pages. You can assign header image and page subheading on any Pages.

![Page Options](_images/page-options.png) 

**Page Header Image**  
Define the header image. You can upload the image or enter a URL. It will display the default solid color (#212526) if there is no header image assigned. You can change the default color from Theme Options (**Theme Options** > **Style** > **Page Hero Header Background Color**).

**Page Subheading**  
Define the subheading text to be displayed below the page title. It's usually a brief description of the page. HTML allowed.

## Featured Image

Featured Image or Post Thumbnail, is an image that is chosen as the representative image for Posts, Pages or Custom Post Types. 

How to assign Images:
1. Navigate to Posts or Page and click on __Set featured image__ at the Featured Image metabox.
2. Upload an image. You can also drag and drop the image from your computer.
3. Click Set __Featured Image__ .

![Reading Setting Post Page](_images/featured-image.png)

?> On blog posts, WordPress will automatically pull the first image to be used as the thumbnail if there is no Featured Image.

?> It is recommended to upload an image that is larger than 640 px.


