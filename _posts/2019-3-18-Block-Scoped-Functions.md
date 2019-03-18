es6 has Block-Scoped Functions.

example:
```js
{
    function a()){
        console.log(5);
    }
    a();
    {
        a();
        function a(){
            console.log(6);
        }
    }

}

```
result:
```
5
6
```

while,
```js
{
    function a(){
        console.log(5);
    }
    a();
    {
        a();
        /*function a(){
            console.log(6);
        }*/
    }

}
```
result:
```
5
5
```