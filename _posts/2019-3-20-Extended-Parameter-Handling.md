
# default parameter values
e.g. ,
```js
function test(a,b,c=2){
    return a+b+c;
}
console.log(test(1,2,3));//6
console.log(test(1,2));//5
```

# rest parameter
it is used in variadic function,e.g.,
```js
function test(a,b,...c){
   let sum=a+b;
   for(let i=0;i<c.length;++i){
       sum+=c[i];
   }
   return sum;
}
console.log(test(1,2,3,4,5));//15
let array=[3,4,5];
console.log(test(1,2,array));//33,4,5
```

>warning:
>rest parameter is a array to contain the rest arguments.But, you should not set a array to the function.as above,the result of <code> test(1,2,array) </code> is wrong. how to solve the problem? you will get the answer from the next section.

# spread operator
spread operator: '<code>...</code>' ,it can spread the elements of collections into iteral elements, e.g.,
```js
function test(a,b,...c){
   let sum=a+b;
   for(let i=0;i<c.length;++i){
       sum+=c[i];
   }
   return sum;
}
console.log(test(1,2,3,4,5));//15
let array=[3,4,5];
console.log(test(1,2,...array));//15
```

# words
1. intuitive:agreeing with waht seems naturally right(without proof or evidence)
2. aggregation:
3. variadic function:it is a function of indefinite arity,i.e.,one which accepts a **variable number of arguments**.
4. arity: in logic,mathmatics,and computer science , **arity** is the number of arguments or operands that the function take.
5. i.e.:that is.
6. e.g.:for example.
7. individual function:

# references
* [Default Parameter Values](http://es6-features.org/#DefaultParameterValues)
* [Rest Parameter](http://es6-features.org/#RestParameter)
* [Spread Operator](http://es6-features.org/#SpreadOperator)