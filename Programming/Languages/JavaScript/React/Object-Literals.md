* Objects can have dynamic / calcuated keys via wrapping the expression in square brackets. For example:

obj = {
    [2+5]: 7
}

console.log(obj[7]);

// returns 7 (or something like that, the key might need to be cast to string)


* Omitting the value in a key/value pair produces the same result has a key/value pair with matching values. For example: 
 obj = {
     seven
 }

 console.log(obj.seven);

 // returns seven
