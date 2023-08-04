## CodePark 10

Desenvolva, utilizando o Google Blockly, um programa que utiliza o nome de um aluno, duas notas e a quantidade de faltas que ele teve. Conclua se o aluno está aprovado ou reprovado de acordo com as especificações:
 
- Se a média do aluno for menor que sete, o sistema deve informar o nome do aluno e que ele está reprovado;
- Se o aluno possuir mais de três faltas, o sistema deve informar o nome do aluno e que ele está reprovado;
- Se a média do aluno for maior ou igual a sete, o sistema deve informar o nome do aluno e que ele está aprovado.

No sistema, todos os valores devem estar armazenados em variáveis.

![image](https://github.com/lizieaz/joyclass_FAP/assets/139813498/cc58709f-9ca9-40f1-91ce-a0d6049aa8e0)

### Resposta

````js

var z, nome, nota1, nota2, faltas;

z = 1;
while (!(z == 0)) {
  nome = window.prompt('Nome do aluno: ');
  nota1 = Number(window.prompt('Primeira nota: '));
  nota2 = Number(window.prompt('Segunda nota: '));
  faltas = Number(window.prompt('Total de faltas:'));
  if ((nota1 + nota2) / 2 < 7 || faltas > 3) {
    window.alert('Aluno reprovado');
  } else {
    window.alert('Aluno aprovado');
  }
  z = Number(window.prompt('Para continuar digite 1, para encerrar digite 0: '));

````
