# Create Hello World Function:

Write a function createHelloWorld. It should return a new function that always returns "Hello World".

___
```
let createHelloWorld = function() {
	return function () {
	return "Hello World"
	}
}
```

primeiro se declara a **_variavel (var, const, let)_** seguida do **_= function(){}_**, se voce quer criar uma funcao dentro de uma funcao pode usar return function () seguido do seu objetivo final.

outra forma de se fazer isso seria utilizando as arrow functions, sendo as mesmas anonimas, a forma seria:

> let createHelloWorld = () => () => "Hello World"

a arrow function (   ()=>  ) sao declaradas para utilizarem um nome de funcao anonima nao declarada, nesse caso:

**_var create = () => {};_** indica o mesmo que **_ var create = function() {return;}_**

___

Creating a "Hello World" function:

First, declare a variable (using var, const, or let) followed by = function() {}. If you want to create a function within a function, you can use return function () followed by your final goal.

Another way to accomplish this is by using arrow functions, which are anonymous by nature. The format would be:

> let createHelloWorld = () => () => "Hello World";

The arrow function syntax () => is used to declare an unnamed, anonymous function. In this context:

> var create = () => {};

indicates the same as:

> var create = function() { return; };

___

##### Final approach for me was: let createHelloWorld = () => () => 'Hello World';
