# testclosure
Learn About Tips and Tricks in Closure

## Description
The reason why i write this code is:

- you can learn about CSS Methodology named BEM (Block, Element Modifier)
- you can learn how to set the position of the element using flexbox, and
- The most important thing is you can learn about tips and trick using CLOSURE. In that loop, we must use Immediately Invoked Function Expression (IIFE) to fill the result with collection of function that return from 1 to the filled value. It because that the i value in that closure is a reference (not a copy) from the outside function, so you must be careful if you use closure inside statement that can change your variable inside the closure (like the loop example). If you want to prove it, you can remove the IIFE like this:

```
    for (var i = 0; i < data; i++) {
        arr[i] = function () {
            return i;
        }
    }
```

This code will make a diffrent result than before (it will print latest i value on each list).Ï
