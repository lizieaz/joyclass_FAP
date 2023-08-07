## CodePark 12

Faça um código, utilizando o Google Blockly, que execute a contagem regressiva de uma bomba, informando o número de segundos para explodir.
Ele deverá mostrar a mensagem “iniciando contagem regressiva”, os segundos passados e, no final, a mensagem “BUM!”.

## Resposta

![image](https://github.com/lizieaz/joyclass_FAP/assets/139813498/72cb6e9c-fe20-4394-832e-b1df5828b799)

````js
var i;

window.alert('Iniciando contagem regressiva');
i = 10;
for (var count = 0; count < 10; count++) {
  window.alert('Contagem regressiva:' + String(i));
  i = i - 1;
}
window.alert('BUM!');
````
