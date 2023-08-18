## Desafio

Você deve criar três listas em JavaScript:
1. para guardar os nomes de dez pessoas;
2. para guardar as suas idades;
3. para guardar as suas cores favoritas.
Em seguida, imprima essas listas. Depois, faça algumas modificações, alterando uma cor e uma idade. Ao terminar, imprima novamente todas as informações das três listas.

````js
const nomes = ['Maria', 'João', 'José', 'Ana', 'Paula', 'Fernando', 'Pedro', 'Cláudia', 'Renato', 'Rafaela'];
const idades = [43, 50, 39, 38, 20, 25, 28, 32, 30, 22];
const cores = ['amarelo', 'vermelho', 'azul', 'rosa', 'preto', 'verde', 'roxo', 'laranja', 'branco', 'marron'];

console.log(`
Listas iniciais

Nomes: ${nomes}
Idades: ${idades}
Cores favoritas: ${cores}`);

idades.splice(1, 1, 31);
cores.splice(2, 1, 'azul claro');

console.log(`
Listas alteradas

Nomes: ${nomes}
Idades: ${idades}
Cores favoritas: ${cores}`);
````
