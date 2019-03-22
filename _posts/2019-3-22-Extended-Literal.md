# Binary & Octal Literal
es6 support intuitive compareing for binary & Octal Literal. e.g.,
```js
console.log(0b11===3);//true
console.log(0o3===3);//ture
```

# Unicode String & RegExp Literal
Extended support using Unicode within strings and regular expressions. e.g. ,
```js
console.log("𠮷".length === 2);//ture
console.log("𠮷".match(/./u)[0].length === 2);//ture
console.log("𠮷" === "\uD842\uDFB7");//ture
console.log("𠮷" === "\u{20BB7}");//ture
console.log("𠮷".codePointAt(0) == 0x20BB7);//ture
for (let codepoint of "𠮷") console.log(codepoint)//𠮷
```

# words
1. Octal:relating to or using a system of numerical notation that has 8 rather than 10 as a base.
2. octal literals:
# reference
1. [Binary & Octal Literal](http://es6-features.org/#BinaryOctalLiteral)
2. [Unicode String & RegExp Literal](http://es6-features.org/#UnicodeStringRegExpLiteral)