# today-i-learned  
#### Repo of stuff I picked up  
---  
## Nov 7
>`indexOf()`  

**Learned from**: [Codewars](https://www.codewars.com/kata/56676e8fabd2d1ff3000000c/solutions/javascript)  
**Lang**: JavaScript  
**Purpose**: Finds the index/position of definted item(s) from an array   
**Example use**:   
```javascript
function findNeedle(haystack) {
  return "found the needle at position " + haystack.indexOf("needle");
}
//or
const findNeedle = haystack => `found the needle at position ${haystack.indexOf('needle')}`;
```

## Nov 9  
>`.` operator  

**Learned from**: [RegexOne](https://regexone.com/)  
**Type**: Regular Expression  
**Purpose**: Wildcard - matches any digit, letter, or whitespace  
**Example use**:  
```javascript
function replaceAny(a) {
  return a.replace(/./g, ' '); //finds any character in the object and replaces it with a space.
}
```

>`@supports`   

**Learned from**: [Aerolab](https://aerolab.co/blog/flexbox-grids/)  
**Lang**: CSS  
**Purpose**: Like a media query, but determines if the browser supports a certain feature.  
**Example use**:
```css
@supports (display: grid) { //checks if broswer supports Grids
  //grid css
}
```

## Nov 14 
>`<inputs>` cannot have `:after`/`:before` pseudo elements  

**Learned from**: [scottohara.me](http://www.scottohara.me/article/pseudo-element-input.html)  
**Lang**: CSS


## Nov 15  
> How to fix the WYSIWYG editor (aka TinyMCE) on Wordpress; hosting permissions

**Learned from**: [Stack Overflow](https://wordpress.stackexchange.com/questions/136738/how-to-fix-a-broken-visual-editor)  
**Type**: Hosting  
**Scenario**: TinyMCE stopped working; visual/text tab stopped responding. Console shows errors associated with TinyMCE's JavaScript. Turns out TinyMCE's php file (`wp-includes/js/tinymce/wp-tinymce.php`) had the wrong permissions. To fix, access host's CPanel and change file's permission to `655`.

## Nov 16  
> CSS Grid  

**Lang**: CSS  
**Purpose**: Layout, templating  
**Resources**:
- Basics - [Mozilla](https://mozilladevelopers.github.io/playground/css-grid)
- References - [Learn CSS Grid](http://learncssgrid.com/)  
- Use cases  
  - [Grid by Example](https://gridbyexample.com/examples/example24/)
  - [CSS-Tricks](https://css-tricks.com/things-ive-learned-css-grid-layout/)
- Use case with Flexbox - [Aerolab](https://aerolab.co/blog/flexbox-grids/)  

## Nov 17  
> `object-fit: fill | contain | cover | none | scale-down`

**Lang**: CSS  
**Purpose**: Determines how a media item fits inside a box.  
**Learned from**: [CSS-Tricks](https://css-tricks.com/almanac/properties/o/object-fit/)

## Nov 27  
> `<?php get_locale() ?>`

**Lang**: PHP (Wordpress)  
**Purpose**: Detects and prints string of current language.  

## Nov 28  
> `filter: drop-shadow()`

**Lang**: CSS  
**Purpose**: Adds a true-to-form drop shadow to objects  
**Learned from**: [CSS-Tricks](https://css-tricks.com/breaking-css-box-shadow-vs-drop-shadow/)  

> `:lang()`

**Lang**: CSS  
**Purpose**: A selector that allows for locale-specific styles.  
**Learned from**: [W3Schools](https://www.w3schools.com/cssref/sel_lang.asp)  
**Example use**: 
```css
//Make paragraphs red if locale/language is Chinese
p:lang(cn) {
  color: red;
}
```

## Dec 5  
> `dir | Rename-Item -NewName {$((get-random).tostring()) + " - " + $_.Name}`

**Type**: Powershell Script  
**Purpose**: Prepends a random number to the original filenames of all files in the directory

## Dec 12
> `@include ('file.structure' . $variable->thing)`

**Lang**: Laravel @ PHP  
**Purpose**: Allows for variables to be passed into an `@include` function  
**Example use**:
```php
    <div class="icon">
        @include ('services.partials.icons.' . $service->slug )
    </div>
    <h3>{{ $service->name }}</h3>
    <p>{{ $service->description }}</p>
```
