# Template Literals
## String interpolation
String interpolation:means you can embed some strings to another string. e.g.,
```js
var customer = { name: "Foo" }
var card = { amount: 7, product: "Bar", unitprice: 42 }
var message = `Hello ${customer.name}, want to buy ${card.amount} ${card.product} for a total of ${card.amount * card.unitprice} bucks?`;
console.log(message);//Hello Foo, want to buy 7 Bar for a total of 294 bucks?
```

while in es5,to achieve this,you must write like this, e.g.,
```js
var customer = { name: "Foo" };
var card = { amount: 7, product: "Bar", unitprice: 42 };
var message = "Hello " + customer.name + "," +"want to buy " + card.amount + " " + card.product + " for" +" a total of " + (card.amount * card.unitprice) + " bucks?";
console.log(message);//Hello Foo,want to buy 7 Bar for a total of 294 bucks?
```

## Custom Interpolation


## Raw String Access


# words
1. Literals: The literal meaning of a word is its original, basic meaning.
2. Interpolation:embed.
3. arbitrary:it is an adjective, mean casual.
4. backslashes: the symbol <code>\\</code> used for separating words or numbers in the names of computer files
# reference

