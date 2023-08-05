## Desafio 11

Desenvolva um código, utilizando o Google Blockly, que utilize as seguintes características de um veículo:
- Quantidade de rodas;
- Peso bruto em quilogramas;
- Quantidade de pessoas no veículo.

Com essas informações, o programa mostrará qual é a melhor categoria de habilitação para o veículo informado a partir das condições:
A: Veículos com duas ou três rodas;
B: Veículos com quatro rodas, que acomodam até oito pessoas e seu peso é de até 3500 kg;
C: Veículos com quatro rodas ou mais e com peso entre 3500 e 6000 kg;
D: Veículos com quatro rodas ou mais e que acomodam mais de oito pessoas;
E: Veículos com quatro rodas ou mais e com mais de 6000 kg.

## Resposta

![image](https://github.com/lizieaz/joyclass_FAP/assets/139813498/c8bd6b61-7073-42c1-ba65-bd6d073a3b2d)

var z, rodas, peso, pessoas;

````js
z = 1;
while (!(z == 0)) {
  rodas = window.prompt('Quantidade de Rodas: ');
  peso = Number(window.prompt('Peso total: '));
  pessoas = Number(window.prompt('Quantidade de Pessoas: '));
  if (rodas < 4) {
    window.alert('Categoria A');
  } else if (peso <= 3500 && pessoas <= 8 && rodas == 4) {
    window.alert('Categoria B');
  } else if (pessoas > 8) {
    window.alert('Categoria D');
  } else if (peso > 6000) {
    window.alert('Categoria E');
  } else if (peso > 3500 && peso <= 6000) {
    window.alert('Categoria C');
  }
  z = Number(window.prompt('Para continuar digite 1, para encerrar digite 0: '));
}
````
