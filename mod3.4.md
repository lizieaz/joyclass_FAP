## Desafio

Crie uma lista encadeada em que cada elemento representa uma pessoa.
Ela precisa conter informações como nome, idade e referência ao filho dela.

## Resposta
````js
const pessoa = [
    ["Robinson", 32, "João"],
    ["Maria", 41, "Pedro"],
    ["Paula", 28, "Julia"],
    ];
    
    for (let i = 0; i < pessoa.length; i++) {
      for (let j = 0; j < pessoa[i].length; j++) {
        console.log(pessoa[i][j]);
      }
    console.log();
    }
````
