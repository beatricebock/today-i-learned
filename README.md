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

