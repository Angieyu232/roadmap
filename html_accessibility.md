# HTML accessibility

<b>Semantic HTML</b> means to use HTML elements according to their intended purpose.

Benefit of Semantic HTML are:

1. easier to develop with
2. better on mobile 
3. good for SEO
4. good for accessibility (screenreader)

## ARIA:  attribute start aria-

attributes that start with aria-* are frequently used with js to keep updated content to screenreaders. 

```
Accessible Rich Internet Applications (ARIA) is a set of attributes that define ways to make web content and web applications (especially those developed with JavaScript) more accessible to people with disabilities.

It supplements HTML so that interactions and widgets commonly used in applications can be passed to assistive technologies when there is not otherwise a mechanism. For example, ARIA enables accessible navigation landmarks in HTML4, JavaScript widgets, form hints and error messages, live content updates, and more. 
```

## ARIA: roles, states and property


  Roles defines a type of user interface element. For instance, alert, banner, button, checkbox, dialog are common ARIA roles.


Authors must assign an ARIA role and the appropriate states and properties to an element during its life-cycle, unless the element already has appropriate ARIA semantics (via use of an appropriate HTML element). 

Here is a sample dialog with accessibility support
```html
<div role="dialog" aria-labelledby="dialog1Title" aria-describedby="dialog1Desc">
   <h2 id="dialog1Title">Subscription Form</h2>
   <p id="dialog1Desc">We will not share this information with third parties.</p>
   <form>
     <p>
       <label for="firstName">First Name</label>
       <input id="firstName" type="text" />
     </p>
     <p>
       <label for="lastName">Last Name</label>
       <input id="lastName" type="text"/>
     </p>
     <p>
       <label for="interests">Interests</label>
       <textarea id="interests"></textarea>
     </p>
     <p>
       <input type="checkbox" id="autoLogin"/>
       <label for="autoLogin">Interests</label>
     </p>
     <p>
         <input type="submit" value="Save Information"/>
     </p>
   </form>
 </div>
```

## Reference and recommended furthur reading:
https://developer.mozilla.org/en-US/docs/Learn/Accessibility/HTML

https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA

https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/ARIA_Techniques