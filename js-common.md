# Build-in browser functions commonly used for Debugging

- getElementsByTagName() : tag name is for instance img, section, href, a
- getElementsByName(), getElementsByClassName(), getElementsById()
- Live NodeList versus Static NodeList:
  - childNode(), getElementsByName() returns live NodeList;
  - QuerySelectorAll() returns static NodeList;
- When getting a NodeList of elements, use functions such as querySelectorAll(), here is a couple examples:

```javascript
var matches = document.querySelectorAll("p");
var container = document.querySelector("#userlist");
var matches = container.querySelectorAll("li[data-active='1']");
```


### JSON
- JSON exist as a string, convert to native JS object easily.
- Both syntax works: obj.keyname and obj[keyname], i.e. superHeroes['members][1]['powers][2]
- Array as JSON also works, accessible using array index
- JSON requires double quotes to be used around string and property names. Single quotes are not valid;
- Validate JSON using application like JSONLint
- JSON.Parse(jsonObj) parse an json object into JS native object
- JSON.stringify() as the name suggest, will take in a json object and convert it into a string



