# 1. array function
## 1.1 expression bodies
if there are no arguments or there are more than 1 argument,you can write like this:
```js
()=>1+1;
(a,b)=>a+b;
```

if there is just an argument,
```js
a=>a+1;
```

but,i think the best way to write arrow function is(having “()”、“{}”、“return"):
```js
(a)=>{
    return a; 
}
```

## 1.2 statement bodies
as above mentioned,you can use "{}" to contain statement bodies.Like this:
```js
(a)=>{
    return a;
}

```

## 1.3 Lexical this
to understand what this point,you can see the article [javaScript的this解惑！](https://blog.csdn.net/wobushixiaobailian/article/details/87613150)

now,back to array function.
>this point current object context

example:
```js
/*in es5*/

let point = {
    x: 0,
    y: 0,
    moveTo: function (x, y) {
        // 内部函数
        let moveX = function (x) {
            this.x = x;//this 绑定到了哪里？
        };
        // 内部函数
        let moveY = function (y) {
            this.y = y;//this 绑定到了哪里？
        };

        moveX(x);
        moveY(y);
    }
};
point.moveTo(1, 1);
console.log(point.x);  //0
console.log(point.y);  //0

```
while,using array function:
```js
/*in es6*/
let point = {
    x: 0,
    y: 0,
    moveTo: function (x, y) {
        // 内部函数
        let moveX = x=> {
            this.x = x;//this 绑定到了哪里？
        };
        // 内部函数
        let moveY =  y=> {
            this.y = y;//this 绑定到了哪里？
        };

        moveX(x);
        moveY(y);
    }
};
point.moveTo(1, 1);
console.log(point.x);  //1
console.log(point.y);  //1

```
--------

# 2. words
1. expression bodies:
2. statement bodies:
3. Lexical:



# 3. reference
[Expression Bodies](http://es6-features.org/#ExpressionBodies)</br>
[Statement Bodies](http://es6-features.org/#StatementBodies)</br>
[Lexical this](http://es6-features.org/#Lexicalthis)
