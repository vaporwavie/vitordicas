Sobre
===================

Hey! O Vitor Dicas consiste em um gerador de palavras. Então basicamente a mágica é um Array composto de um banco de frases prontas do nosso amigo Vitor e que são ordenados aleatoriamente.

Como Funciona
===================


> **Dica**: Considere que este script deverá subsituir um texto de uma determinada Div na página, como é colocado abaixo.
```
<!-- Div para o gerador -->
<div>
        <h4 class="center black-text" id="geradica">SUA DICA AQUI </h4> <br>
      <button class="btn waves-effect waves-light" type="button" onclick="vitorDicas()">GERAR DICA</button>
  </div>
```

> **Dica**: O Array pode ser usado de diversos modos, aleatório, não-aleatório e afins. Nesta situação, o modelo está em ordem comum.
```
// Array de dicas
var arrayDicas=['Traz comida', 'Vei', 'Vem estudar aqui na RUY 2h30', 'Biquinho', 'Marcos tá te procurando', '310b',
    'Cabe +1?', 'Cadê titia', ':D', 'Aquela menina é feia vei', 'Trouxe lanche?', 'Vamos estudar domingo 14h',
    'Vai dormir rapaz', 'Os melhores cafés sempre são os grátis', 'Vamos embora vei']
```

> **Dica**: Shift e Push precisam estar no código para a ordem do Array. 
```
// Condição que vai substituir e gerar uma dica na Div identada
function vitorDicas() {
    var value = arrayDicas[Math.floor(Math.random() * Math.random() * arrayDicas.length)];
    var value = arrayDicas.shift();
    arrayDicas.push(value);
    document.getElementById("geradica").innerHTML=value;
}
```

Publicidade e Contato
==========================
  luizaugusto@linuxmail.org
