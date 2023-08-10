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

var
voto, candidato_X, candidato_Y, candidato_Z, brancos: inteiro

inicio

escreval("Votação iniciada")
escreval("Candidatos disponíveis:")
escreval("Candidato X: Número 889")
escreval("Candidato Y: Número 447")
escreval("Candidato Z: Número 515")

z=1

enquanto z==1 faca
    escreval("Registre seu voto:")
    leia(voto)

    se voto==889 entao
        canditado_X = candidato_X + 1
        senao se voto == 447 entao
        candidato_Y = candidato_Y + 1
        senao se voto == 515 entao
        candidato_Z = candidato_Z + 1
        senao
        brancos = brancos + 1
    fimse

    escreval("Para encerrar a votação, digite 0")
    leia(z)
fimenquanto

escreval("Resultado da votação")
se candidato_X > canditato_Y entao
vencedor = candidato_X
senao se candidato_Z > candidato_X entao
vencedor...





## Resposta
````js
let votoCandidato = {
    candidato_X: 889,
    candidato_Y: 847,
    candidato_Z: 515,
    branco: 0,
    nulo: 0
}

while (true) {
   let escolhaDeCandidato = parseInt(prompt("Votação 2023.\nCAndidatos disponíveis\n\nCandidato 1 - 889\nCandidato 2 - 847\nCandidato 3 - 515\nPara votar em branco - Vote 0"))

   if (isNaN(escolhaDeCandidato)){
        alert('Voto inválido. Tente Novamente.')
        continue
    } else if(escolhaDeCandidato == 889){
        alert('Você votou no candidato 1!')
        votoCandidato.candidato_X++
    } else if(escolhaDeCandidato == 847){
        alert('Você votou no candidato 2!')
        votoCandidato.candidato_Y++
    } else if(escolhaDeCandidato == 515){
        alert('Você votou no candidato 3!')
        votoCandidato.candidato_Z++
    } else if(escolhaDeCandidato == 0){
        alert('Você votou em branco.')
        votoCandidato.branco++
    } else{
        alert('Você votou nulo.')
        votoCandidato.nulo++
    }

        let maioriadeVotos = Math.max(votoCandidato.candidato_X,votoCandidato.candidato_Y,votoCandidato.candidato_Z,votoCandidato.branco,votoCandidato.nulo)
        let candidatoGanhador
        
        if (maioriadeVotos == votoCandidato.candidato_X){
        candidatoGanhador = "Candidato 1!"
        } else if (maioriadeVotos == votoCandidato.candidato_Y){
        candidatoGanhador = "Candidato 2!"
        } else if (maioriadeVotos == votoCandidato.candidato_Z){
        candidatoGanhador = "Candidato 3!"
        } else if (maioriadeVotos == votoCandidato.branco){
        candidatoGanhador = "Votos em branco."
        } else{
        candidatoGanhador = "Votos nulos"
        }

    let continuarVoto = parseInt(prompt("Deseja encerrar a votação?\n1 - Sim\n2 - Não"))
    if (continuarVoto == 1){
            alert('Votações encerradas.')
            alert('Contabilizando votos...')
            alert('Computando resultados...')
            alert('Votação conluída!')
        alert(`Candidato vencedor: ${candidatoGanhador}\n\nTotal de votos:\n\nCandidato1 - ${votoCandidato.candidato_X}\nCandidato 2 - ${votoCandidato.candidato_Y}\nCandidato 3 - ${votoCandidato.candidato_Z}\nVotos brancos - ${votoCandidato.branco}\nVotos nulos - ${votoCandidato.nulo}`)
        break
    } else if (continuarVoto != 2) {
        alert('Opção inválida.')
    }
}````
