
# constant
what is constant?
the constant cannot be re-assigned new content(just like the constant of java language).
>warning:you cann't alter the value of the constan,but you can alter its assigned vale.

example:
```js
const a={"a":1,"b":2};
console.log(a);
a.a=3;//okay
console.log(a);

a={"a":12,"b":12};//fail,TypeError: Assignment to constant variable.
```

# words
1. immutable:unable to be changed

# references
[ECMAScript 6 Contant](http://es6-features.org/#Constants)