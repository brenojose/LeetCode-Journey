# Closure
Quando uma função lembra seu escopo léxico, mesmo quando a função é executada fora desse escopo.

Por exemplo:

closure.js
```
function fora() {
    let x = 50;
    function dentro() {
        return x + 3;
    }
    return dentro;
}
```

### Conclusão
Closures são poderosas porque permitem que funções "lembrem" do ambiente em que foram criadas, proporcionando acesso contínuo a essas variáveis mesmo quando a função é executada em um contexto diferente. Se precisar que variáveis de outros arquivos sejam acessíveis, passe-as como argumentos para manter o comportamento esperado.

___

When a function remembers its lexical scope, even when the function is executed outside that scope.

For example:

closure.js
```
function outside() {
    let x = 50;
    function inside() {
        return x + 3;
    }
    return inside;
}
```
Conclusion
Closures are powerful because they allow functions to "remember" the environment in which they were created, providing continuous access to those variables even when the function is executed in a different context. If you need variables from other files to be accessible, pass them as arguments to maintain the expected behavior.
