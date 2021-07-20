# testesAutomatizados-Calculadora-Windowns7
 
<p>Para utilização do script é necessario realizar a instalação da versão da calculadora do <b>windowns 7</b> anexado ao repositório.</p>

<p>Realizada a instalação, inicie o projeto com o TestComplete e passe uma **string** contendo o cálculo desejado para a função **calcular**</p>

```
function teste() {
  Log["AppendFolder"]('Testes')
  Calculadora_IniciarCalculadora();
  calcBotoes('ce');
  calcular('10*2=20');
  Log["PopLogFolder"]();
}
```
 
 A função calcBotoes efetua o clique no botão desejado e podem ser mapeados novas opções caso desejado
 
 A função calcular recebe uma string efetua os cliques de acordo com sua posição na string e verifica se o valor representado no visor da string é igual ao valor passado após o "="
