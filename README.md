# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.


# I rewrote it for clarity
```javascript
function mystery(a) {
    if (a.length == 1) {
        return a[0];
    }
    var foo = mystery(a.slice(1, a.length))

    if (foo > a[0]) {
        return foo;
    }
    else {
        return a[0];
    }
}
```

The "mystery" function seems to use recursion to find the single largest character value in the input. it does not take an empty input such as "".
If i entered 13 for example it would output 3, aswell as if i entered 31. because 3 holds the largest value. 
It works for string characters aswell, so if i entered AiDanN because n has the larget ascii value the output would be "n", i just looked up a ascii table n = 110 while N = 78.
