## Desafio

Desenvolva um código que simule uma eleição com três candidatos.
- candidato_X => 889
- candidato_Y => 847
- candidato_Z => 515
- branco => 0

O código deve perguntar se deseja finalizar a votação depois do voto. Caso o número do voto não corresponda a nenhum candidato ou seja branco, ele deve ser tratado como nulo. Se for inserido um texto ao invés de número, o código deve retornar uma mensagem para votar novamente.

Quando a votação for finalizada, o código deverá mostrar o vencedor, aquele com o maior número de votos e, também, a quantidade de votos de cada candidato, os brancos e nulos. 

## Resposta

< em construção >
````
Algoritmo "Votacao"

Var
// Seção de Declarações das variáveis 
voto, x, y, z, brancos, n: inteiro

Inicio
// Seção de Comandos, procedimento, funções, operadores, etc... 

escreval("Votação iniciada")
escreval("Candidatos disponíveis:")
escreval("Candidato X: Número 889")
escreval("Candidato Y: Número 447")
escreval("Candidato Z: Número 515")

n<-1

enquanto n=1 faca
escreval("Registre seu voto:")
leia(voto)

se voto=889 entao
    x <- x + 1
    senao se voto == 447 entao
    y <- y + 1
    senao se voto == 515 entao
    z <- z + 1
    senao
    brancos <- brancos + 1
fimse

escreval("Para encerrar a votação, digite 0, para continuar digite 1")
leia(n)
fimenquanto

Fimalgoritmo
````
