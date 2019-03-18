es6 has block scoped variables.
example,in es5
```js
for(var i=0;i<5;++i){
    console.log(i);
}
console.log(i);
```
result
```
0
1
2
3
4
5
```

while in es6:
```js
for(let i=0;i<5;++i){
    console.log(i);
}
console.log(i);

```
result:
```
0
1
2
3
4
/home/fengli/Desktop/blog/fenglier.github.io/_posts/test.js:4
console.log(i);
            ^

ReferenceError: i is not defined
    at Object.<anonymous> (/home/fengli/Desktop/blog/fenglier.github.io/_posts/test.js:4:13)
    at Module._compile (internal/modules/cjs/loader.js:689:30)
    at Object.Module._extensions..js (internal/modules/cjs/loader.js:700:10)
    at Module.load (internal/modules/cjs/loader.js:599:32)
    at tryModuleLoad (internal/modules/cjs/loader.js:538:12)
    at Function.Module._load (internal/modules/cjs/loader.js:530:3)
    at Function.Module.runMain (internal/modules/cjs/loader.js:742:12)
    at startup (internal/bootstrap/node.js:283:19)
    at bootstrapNodeJSCore (internal/bootstrap/node.js:743:3)
```