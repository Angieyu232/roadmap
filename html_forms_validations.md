## HTML Forms and Validations

To provide server with valid user data and prevent malicious user from sending erroneous data to overload the server, client-side validation is strongly recommended.

HTML5 has build-in form validations, which means html along can validate most user data without relying in JavaScript. To recap form control, here are some useful attr: 

```
* required: Specifies whether a form field needs to be filled in before the form can be submitted.
* minlength and maxlength: Specifies the minimum and maximum  length of textual data (strings)
* min and max: Specifies the minimum and maximum values of numerical input types
* type: Specifies whether the data needs to be a number, an email address, or some other specific preset type. 
* pattern: Specifies a regular expression that defines a pattern the entered data needs to follow.

```

Here is a sample bootstrap form-group that prompt warning message when fields are not valid with <em>required</em> and <em>minlength</em> attr: 



```html
<form>
  <div class="form-group">
   <label for="exampleInputEmail1">Email address :</label>
    <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" required="true" placeholder="Enter email">
  </div>
  <div class="form-group">
    <label for="exampleInputPassword1">Password: </label>
    <input type="password" class="form-control" id="exampleInputPassword1" required="true" minlength="6" placeholder="Password">
  </div>
  <div class="form-check">
    <input type="checkbox" class="form-check-input" id="exampleCheck1">
    <label class="form-check-label" for="exampleCheck1">Check me out</label>
  </div>
  <button type="submit" class="btn btn-primary">Submit</button>
</form>
```


### Reference: 
https://developer.mozilla.org/en-US/docs/Learn/Forms/Form_validation