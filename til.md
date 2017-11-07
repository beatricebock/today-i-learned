# today-i-learned  
#### Repo of stuff I picked up  
---  
## Nov 7
`indexOf()`  
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

