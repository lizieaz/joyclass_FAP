## Desafio

Faça, utilizando o Google Blockly, uma função calculadora que os números e as operações serão feitas pelo usuário. O código deve ficar rodando infinitamente até que o usuário escolha a opção de sair. No início, o programa mostrará a seguinte lista de operações:
1: Soma
2: Subtração
3: Multiplicação
4: Divisão
0: Sair

Digite o número para a operação correspondente e caso o usuário introduza qualquer outro, o sistema deve mostrar a mensagem “Essa opção não existe” e voltar ao menu de opções.

Após a seleção, o sistema deve pedir para o usuário inserir o primeiro e segundo valor, um de cada. Depois precisa executar a operação e mostrar o resultado na tela. Quando o usuário escolher a opção “Sair”, o sistema irá parar. 

## Resposta

![image](https://github.com/lizieaz/joyclass_FAP/assets/139813498/5bd9febd-f79b-40b3-97c4-5702b3167cfa)

````js
var operacao, n1, n2;

operacao = 1;
while (operacao != 0) {
  window.alert('Para iniciar, escolha uma das operações:');
  operacao = window.prompt('1: Soma 2: Subtração 3: Multiplicação 4: Divisão 0: Sair');
  if (operacao == 1) {
    n1 = Number(window.prompt('Digite o primeiro número: '));
    n2 = Number(window.prompt('Digite o segundo número: '));
    window.alert('Resultado da soma: ' + String(n1 + n2));
  } else if (operacao == 2) {
    n1 = Number(window.prompt('Digite o primeiro número: '));
    n2 = Number(window.prompt('Digite o segundo número: '));
    window.alert('Resultado da subtração: ' + String(n1 - n2));
  } else if (operacao == 3) {
    n1 = Number(window.prompt('Digite o primeiro número: '));
    n2 = Number(window.prompt('Digite o segundo número: '));
    window.alert('Resultado da multiplicação: ' + String(n1 * n2));
  } else if (operacao == 4) {
    n1 = Number(window.prompt('Digite o primeiro número: '));
    n2 = Number(window.prompt('Digite o segundo número: '));
    window.alert('Resultado da divisão: ' + String(n1 / n2));
  } else if (operacao == 0) {
    window.alert('Programa encerrado');
  } else {
    window.alert('Essa opção não existe');
  }
}
````
