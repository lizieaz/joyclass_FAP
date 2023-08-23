## Desafio

Temos o array [15, 8, 10, 25, 12, 30, 5, 20, 18, 7] e precisamos criar um código em JavaScript para encontrar o valor 20.
Para isso, temos que escolher entre realizar uma busca linear ou binária de acordo com a que for mais adequada para essa situação.
Codifique a solução mais eficiente para buscar o número 20 no array.

## Resposta
![image](https://github.com/lizieaz/joyclass_FAP/assets/139813498/a7a73706-30a2-4b92-9552-b590d88bf364)


````js
function buscar(array, buscado) {
    for (let i = 0; i < array.length; i++) {
        if (array[i] === buscado) {
            console.log(`O elemento igual a ${buscado} está na posição ${i} do array`)
        }
    }
    console.log("Elemento não encontrado")
}

const numeros = [15, 8, 10, 25, 12, 30, 5, 20, 18, 7];

buscar(numeros, 30);
````
