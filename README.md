# vt-toggle
Turn HTML checkbox inputs into fancy toggle switches with just a CSS class


**Demo**: https://victornpb.github.io/vt-toggle/


# What is this?

You can turn a simple checkbox like this

> <img src="http://i.imgur.com/X64C7Ab.png">

Into this fancy toggle just by addind the `vt-toggle` class
  
> <img src="http://i.imgur.com/ZlP9PV7.png"> 


    <input type="checkbox" class="vt-toggle">
   

# Install

Ok, cool! how can I get it?

#### [NPM](https://www.npmjs.com/package/vt-toggle) 

    npm install vt-toggle

#### Bower

    bower install vt-toggle
    
#### CDN

    https://unpkg.com/browse/vt-toggle@1.0.1/css/vt-toggle.css
    
#### Download

    https://github.com/victornpb/vt-toggle/releases/
### Importing into project

#### Import using link
```html
<link rel="stylesheet" type="text/css" href="bower_components/vt-toggle/css/vt-toggle.css">
<link rel="stylesheet" type="text/css" href="node_modules/vt-toggle/css/vt-toggle.css">
```
##### Import using SASS
```css
@import "node_modules/vt-toggle/scss/vt-toggle"; // NPM
@import "bower_components/vt-toggle/scss/vt-toggle"; // Bower
```

### Creating your own classes using SASS

You can create your own classes using the SASS mixin.
```scss
@mixin vt-toggle($toggleWidth, $toggleHeight, $handleMargin, $roundness, $on-color, $off-color, $label)
```

Example:
```scss
@import "bower_components/vt-toggle/scss/vt-toggle";

$blue: #00f;
$red: #f00;

input.vt-toggle.accent {
    @include vt-toggle(44px, 22px, 1px, 1, $blue, gray, false);
}
input.vt-toggle.danger {
    @include vt-toggle(44px, 22px, 1px, 1, $red, gray, false);
}
```

Then you can use:
```html
<input type="checkbox" class="vt-toggle accent"> I'm blue toggle
<input type="checkbox" class="vt-toggle danger"> I'm red toggle
``` 
----

# Default styles

## Default Sizes:

| class | Dimensions      | Preview                                    |
|-------|-----------------|--------------------------------------------|
| xs    | 18x22           | <img src="http://i.imgur.com/sj72uAN.png"> |
| sm    | 32x16           | <img src="http://i.imgur.com/K5qZgg7.png"> |
| md    | 44x22 (default) | <img src="http://i.imgur.com/ofj7u7E.png"> |
| lg    | 64x32           | <img src="http://i.imgur.com/PKHziIP.png"> |

## States

| State          | Preview                                    |
|----------------|--------------------------------------------|
| On             | <img src="http://i.imgur.com/ofj7u7E.png"> |
| Off            | <img src="http://i.imgur.com/fMIYHt9.png"> |
| Disabled (on)  | <img src="http://i.imgur.com/82rzSlS.png"> |
| Disabled (off) | <img src="http://i.imgur.com/jXcJQql.png"> |
