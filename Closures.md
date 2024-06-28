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