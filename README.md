# Web Dev Notes
notes on  Web Development and  CS fundamentals


### Javascript Tips
- "use strict" can massively improve performance and prevent semantic errors 
- for javascript, use **typeof** function to avoid type cast error
- understand the three declaration keywords: var, let, const, for memory optimization and better performance, use let and const as much as possible, for the latter two are block-scope and local
- double equals (==) are loose equals, i.e 3 == '3' => true; While triple equals ( === ) returns true if both operands are of the same type and value
- For falsy value comparison, try it in console or refer to https://codeburst.io/javascript-showdown-vs-7be792be15b5
- for best practice and readability, use bracket with conditions and loops

```javascript
if (condition_1) {
  statement_1;
} else if (condition_2) {
  statement_2;
} else if (condition_n) {
  statement_n;
} else {
  statement_last;
} 
```
- it's also possible to assign value in condition statement
```javascript
if ((x = y)) {
  /* statements here */
}
/* OR assign a function */
if ((x = somefunction())) {
  alert(x)
 }
```
```javascript
for (let i in arr) {
   console.log(i); // logs "0", "1", "2", "foo"
}
```


