# Shortcodes

Camden theme comes with shortcodes which allow you to create more customized post and page layouts with the help of columns, buttons, lists, etc.

Briefly, shortcode is a special tag that you can enter into a post that gets replaced with different content when actually viewing the post on the website. You can add the shortcodes from the WordPress visual editor. Navigate to a Post or a Page, and find the Shortcode Editor button in the post editor window.

![Shortcode Button](_images/shortcode-button.png)

## Grid
The grid shortcode in Camden theme is based on 12-column [Foundation Grid system](https://foundation.zurb.com/sites/docs/grid.html).

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

### 1/3 & 2/3 Columns
```html
[one_third_alpha] ... [/one_third_alpha]
[two_third_omega] ... [/two_third_omega]
```

### 2/3 & 1/3 Columns
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
 ```
 
 



## Typography
### Check List
### Check List Circle
### Left Pull Quotes
### Right Pull Quotes
### Blockquote

## Media
### Orbit
This is a shortcode to create Orbit responsive slider. It has similar attributes we used in the Clearing shortcode.


Placing [orbit] in your editor creates a responsive slider from all the images attached to the post/page

Attributes:
id — takes a post/page ID, defaults to current post/page
size — size of the images used, defaults to large
include — list of attachment IDs to include
exclude — list of attachment IDs to exclude
How To Use Shortcode Attributes:
Adding attribute to the [orbit] shortcode looks like this: [orbit size="small"]. Adding a second attribute would look as follows: [orbit size="small" exclude="6,3,1"]. It’s only necessary to add a attribute to the shortcode if you wish to override the default attribute.
### Reveal
This is a shortcode to create simple modal windows on your site.

[reveal link="Link text" linkclass="button radius alert"]…[/reveal]
Attributes:
link — button or link text
linkclass — additional CSS classes on the button
class — additional CSS classes on the modal window
## Accordion
## Tabs
## Vertical Tabs
## Callout
The [alert]…[/alert] shortcode gives you and your editors and easy way to display the Foundation Alerts with some additional options.
Attributes

Alert boxes come with two additional options: close=no (default is yes) and timeout=2000 (timeout in ms). The timeout option makes the box disappear after the timer is done.

## Tooltip
This is a shortcode that creates simple Tooltips.

Attributes:
position — top | bottom | left | right
title — Text in the tip
class — Additional CSS classes.
width — Size of the tip, in pixels.
## Button
```html
[btn url="#" type="basic"] Basic Button [/btn]
[btn url="#" type="hollow"] Hollow Button [/btn]
[btn url="#" type="action"] Action Button [/btn]
```
![Shortcode Grid](_images/shortcode-button-type.png)

![Shortcode Grid](_images/shortcode-button-color.png)
