## Desafio

Nesta atividade, você deve criar um código em JavaScript com uma matriz bidimensional para armazenar informações sobre animais e as suas características.
Cada linha deve representar um animal e cada coluna terá as diferentes informações sobre ele, como nome, espécie e idade.

````js
const animais = [
    ['totó', 'cachorro', 2],
    ['tatá', 'passarinho', 1],
    ['titi', 'gato', 3]
];

for (let i = 0; i < animais.length; i++) {
    for (let j = 0; j < animais.length; j++) {
        console.log(animais[i][j]);
    }
}
````
