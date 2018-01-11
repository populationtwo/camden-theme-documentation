# Shortcodes

Camden theme comes with shortcodes which allow you to create a more customized post and page layouts with the help of columns, buttons, lists, etc.

Briefly, a shortcode is a special tag that you can enter into a post that gets replaced with different content when actually viewing the post on the website. You can add the shortcodes from the WordPress visual editor. Navigate to a Post or a Page, and find the Shortcode Editor button in the post editor window.

!> NOTE: The shortcodes features requires [Camden Add-ons](https://github.com/populationtwo/camden-add-ons ":target=_blank") plugin.
 
![Shortcode Button](_images/shortcode-button.png)

## Grid
The grid shortcode in Camden theme is based on 12-column [Foundation Grid system](https://foundation.zurb.com/sites/docs/grid.html ":target=_blank").

![Shortcode Grid](_images/shortcode-grid.png)

### 2 Columns

```html
[one_half_alpha] ... [/one_half_alpha]
[one_half_omega] ... [/one_half_omega]
```

### 3 Columns
```html
[one_third_alpha] ... [/one_third_alpha]
[one_third] ... [/one_third]
[one_third_omega] ... [/one_third_omega]
```

### 4 Columns
```html
[one_fourth_alpha] ... [/one_fourth_alpha]
[one_fourth] ... [/one_fourth]
[one_fourth] ... [/one_fourth]
[one_fourth_omega] ... [/one_fourth_omega]
```

### <sup>1</sup>/<sub>3</sub> & <sup>2</sup>/<sub>3</sub> Columns
```html
[one_third_alpha] ... [/one_third_alpha]
[two_third_omega] ... [/two_third_omega]
```

### <sup>2</sup>/<sub>3</sub> & <sup>1</sup>/<sub>3</sub> Columns
```html
[two_third_alpha] ... [/two_third_alpha]
[one_third_omega] ... [/one_third_omega]
```

### Custom
Custom size grid offer more control of the grid layout. The sum of sizes of all columns started with the first and ended with the last column must not exceed 12.
 
 ```html
[column columns=12]...[/column]

[column columns=7]...[/column][column columns=5]...[/column]

[column columns=3]...[/column][column columns=3]...[/column][column columns=6]...[/column]

[column columns=10 offset=2 class="optional-class"]...[/column]

```
 
 Attributes:
 - `columns` — grid columns size. Acceptable values are `1` to `12`.
 - `offset` — pushes the column to the right. Acceptable values are `1` to `12`.
 - `class` —  optional CSS classes.
 



## Typography
### Checklist

![Checklist](_images/shortcode-checklist.png)

```html
[checklist]
<ul>
 	<li>Item 1</li>
 	<li>Item 2</li>
 	<li>Item 3</li>
</ul>
[/checklist]
```

### Checklist Circle

![Checklist Circle](_images/shortcode-checklist-circled.png)

```html
[checklist_circled]
<ul>
    <li>Item 1</li>
 	<li>Item 2</li>
 	<li>Item 3</li>
</ul>
[/checklist_circled]
```

### Left Pull Quote

![Left Pull Quote](_images/shortcode-blockquote-left.png)

```html
[pullquote_left] Lorem ipsum [/pullquote_left]
```

### Right Pull Quote

![Right Pull Quote](_images/shortcode-blockquote-right.png)

```html
[pullquote_right] Lorem ipsum [/pullquote_right]
```

### Blockquote

![Blockquote](_images/shortcode-quote.png)
```html
[quote] Lorem ipsum [/quote]

[quote] Lorem ipsum <br><cite>John Doe</cite> [/quote]
```

## Media

### Orbit
This is a shortcode to create Orbit responsive slider. 

Placing `[orbit]` in your editor creates a responsive slider from all the images attached to the post or page

![Orbit slider](_images/shortcode-orbit-slider.png)

```html
[orbit] // Display all images attached to current post/page
[orbit exclude="1"] // Display all images attached to current post/page except image with ID 1.
[orbit include="1,2,3"] // Display images ID 1,2, & 3.
[orbit size="small"] // Use small image
```

Attributes:
- `id` — takes a post/page ID, defaults to current post/page
- `size` — size of the images used, defaults to `large`
- `include` — list of attachment IDs to include
- `exclude` — list of attachment IDs to exclude

?> It’s only necessary to add a attribute to the shortcode if you wish to override the default attribute.

How To Attach Image to Current Post/Page:
1. Go to __Edit Post__ or __Edit Page__.
2. Click __Add Media__
3. Go to __Insert Media__ > __Upload Files__ tab and upload the image files. Add the image caption accordingly. Click __Insert into post__ afterward.
4. You will see duplicate images from the attached image and orbit slider in the post/page. Once you see the Orbit slider, you can delete the attached image from post/page.

### Reveal
Reveal shortcode displays simple modal windows on your site. A modal is a container where you can put any kind of content inside it, from text to forms to video.

![Reveal modal](_images/shortcode-reveal.png)

```html
// Basic shortcode
[reveal link="link text"]
Modal window content
[/reveal]

// Shortcode with all the attributes
[reveal link="link text" linkclass="button-basic button secondary" class="large"]
Modal window content
[/reveal]
```

Attributes:
- `link` — Link or button text (required).
- `linkclass` — Additional CSS classes on the button. 
- `class` — Optional CSS classes on the modal window. The size of a modal can be changed with sizing classes (`tiny`, `small`, `large` and `full`).

## Accordion

Accordions are elements that help you navigate multiple contents in a single container. They can be used for switching between items in the container.

![Accordion](_images/shortcode-accordion.png)

```html
[accs class="optional-class"]
[acc active="is-active" title="Accordion 1"]Accordion pane 1 content[/acc]
[acc title="Accordion 2"]Accordion pane 2 content[/acc]
[acc title="Accordion 3"]Accordion pane 3 content[/acc]
[/accs]
```
Attributes:
- `title` — Title of the accordion pane (required).
- `active` — Set the active accordion pane (required).
- `class` — Optional CSS classes.

## Horizontal Tabs
Tabs are elements that help navigate multiple contents in a single container. They can be used for switching between items in the container.

![Tabs](_images/shortcode-h-tab.png)

```html
[tabs class="optional-class"]
[tab title="Tab 1 Title" active="is-active"] Tab 1 content [/tab]
[tab title="Tab 2 Title"] Tab 2 content [/tab]
[tab title="Tab 3 Title"] Tab 3 content [/tab]
[/tabs]
```

Attributes:
- `title` — Title of the tab (required).
- `active` — Set the active tab (required).
- `class` — Optional CSS classes.

## Vertical Tabs

Tabs can be aligned vertically using Vertical Tabs.

![Tabs](_images/shortcode-v-tab.png)

```html
[vtabs class="optional-class"]
[vtab title="Tab 1 Title" active="is-active"] Tab 1 content [/vtab]
[vtab title="Tab 2 Title"] Tab 2 content [/vtab]
[vtab title="Tab 3 Title"] Tab 3 content [/vtab]
[/vtabs]
```

Attributes:
- `title` — Title of the tab (required).
- `active` — Set the active tab (required).
- `class` — Optional CSS classes.


## Callout
Callout shortcode gives you and your editors and easy way to display panel or alert box with some additional options.

![Shortcode Callout Dialog](_images/shortcode-callout-dialog.png)
![Shortcode Callout](_images/shortcode-callout.png)

```html
// Default callout
[callout] Lorem ipsum [/callout] 

// Callout without close button
[callout close=no] Lorem ipsum [/callout]

// Success callout
[callout type="success"] Lorem ipsum [/callout]
```

Attributes:
- `type` — Appearance of a callout. Can be `standard`, `success`, `warning`, `alert`, `primary`, or `secondary`.
- `close` — Set to `no` to disable close button.


## Tooltip
This is a fairly simple shortcode that creates simple [Tooltip](https://foundation.zurb.com/sites/docs/tooltip.html ":target=_blank"). 

![Shortcode Tooltip](_images/shortcode-tooltip.png)

```html
[tooltip title="Tooltip content"]Lorem ipsum[/tooltip]
[tooltip position="top" title="Tooltip content" class="optional-class"]Lorem ipsum[/tooltip]
```

Attributes:
- `position` — Position of tooltip. Can be `left`, `right`, `bottom`, `top`, or `auto`.
- `title` — Text / content of tooltip.
- `class` — Optional CSS classes.


## Button
![Shortcode Button Dialog](_images/shortcode-button-dialog.png)

__Types__

![Shortcode Button Types](_images/shortcode-button-type.png)

__Color__

![Shortcode Button Color](_images/shortcode-button-color.png)

__Size__

![Shortcode Button Size](_images/shortcode-button-sizes.png)

__Arrow__

![Shortcode Button Arrow](_images/shortcode-button-arrow.png)


Minimal shortcode:
```html
// Basic shortcode
[btn url="https://envato.com"]Button[/btn]

//Shortcode with all its attributes:
[btn url="https://envato.com" type="action" color="primary" target="_blank" arrow="true" size="large"]
Button
[/btn]
```

Attributes:
- `type` — button type. It can be `basic`, `hollow`, or `action`. The default type is `basic`, or without type attribute.
- `color` — button color. It can be `primary`, `secondary`, `red`, `orange`, `yellow`, `green`, `blue`, or `teal`. Default color is grey, without a `color` attribute.        
- `size` — button size. It can be `small` or `large`. The default size is `normal`.
- `target` — specifies where to display the linked URL. Set `_blank` to open URL in a new tab.
- `arrow` — set arrow attribute to `false` to disable the arrow. Arrow is enabled by default.                                 