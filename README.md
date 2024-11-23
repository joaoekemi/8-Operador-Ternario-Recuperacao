# Operador Condicional Ternário

A última estrutura de condição que estudaremos será o operador ternário. Este traz algumas melhorias em relação ao If Else e o Switch Case, mas também possui algumas desvantagens.

Eis o link da documentação oficial: https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Operators/Conditional_operator


## Estrutura

Dentro todas as estruturas de condição, o operador ternário é o que possui a estrutura mais simples, mas igualmente é essencial observar os caracteres e suas posições: 

``` condição ? saida_1 : saida_2 ```

- A ```condição```, como de costume será o que queremos validar.
- O símbolo de interrogação ```?``` é parte essencial da estrutura e pode ser interpretada como uma pergunta, se a condição for verdadeira, então...
- A ```saida_1``` representa a primeira resposta da pergunta, do que tentamos validar.
- Enquanto que a ```saida_2``` reprenta a segunda resposta da pergunta.


## Ternário e Outras Estruturas de Condição

Vale ressaltar que diferente das outras estruturas de condição onde é possível utilizar uma ou elas mesmas dentro delas, o operador ternário não aceita muito bem essa dinâmica, ex:

```
condição ? if (condição) {} : switch (condição) {}
```
```
hemisferio == N ? ( if (mes == 1) {} ) : ( switch (mes) {} )
```

Mesmo utilizando um agrupador como ```{}``` ou ```()``` essa relação, neste formato não irá funcionar.

Mas utilizar as expressões ```&&``` (e), ```||``` (ou) para realizar mais de uma comparação para a mesma saída, ainda é possível. Ex:

``` condição && condição ? saida_1 : saida_2 ```

Ou

``` condição || condição || condição ? saida_1 : saida_2 ```