# Shortcodes

Camden theme comes with shortcodes which allow you to create more customized post and page layouts with the help of columns, buttons, lists, etc.

Briefly, shortcode is a special tag that you can enter into a post that gets replaced with different content when actually viewing the post on the website. You can add the shortcodes from the WordPress visual editor. Navigate to a Post or a Page, and find the Shortcode Editor button in the post editor window.

![Shortcode Button](_images/shortcode-button.png)

## Grid
The grid in Camden theme is based on [Foundation Grid](https://foundation.zurb.com/sites/docs/grid.html). This shortcode can create most used predefined layout. You can get more control of the grid layout by using the [Foundation Grid Columns shortcode](/shortcodes?id=grid-columns).

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
## Typography
### Check List
### Check List Circle
### Left Pull Quotes
### Right Pull Quotes
### Blockquote

## Media
### Orbit
### Reveal

## Accordion
## Tabs
## Vertical Tabs
## Callout
## Tooltip
## Button
```html
[btn url="#" type="basic"] Basic Button [/btn]
[btn url="#" type="hollow"] Hollow Button [/btn]
[btn url="#" type="action"] Action Button [/btn]
```
![Shortcode Grid](_images/shortcode-button-type.png)

![Shortcode Grid](_images/shortcode-button-color.png)
