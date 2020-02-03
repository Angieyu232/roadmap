


## Exercises

 1. write a js function to find palidrome string;
    ```javascript
    function isPalindrome (str) { 
        let i= 0; j = str.length-1;  
        while (i != j) { 
            if(str.charAt[i]!=str.charAt[j]) { return false; } 
            str = str.slice(i, j); i++; j--;
        } 
        
        return true;
    }
    ```



 2. 
