# Caderno virtual de JavaScript <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/99/Unofficial_JavaScript_logo_2.svg/1200px-Unofficial_JavaScript_logo_2.svg.png" height="45" width="45">


## Exibir Mensagens
### console.log() exibe mensagem no console do navegador
```js
console.log("Hello, Word")// irá exibir "Hello, Word" no console do navegador
```
### document.write() exibe a mensagem diretamenta na página(usado junto com html)
```js
document.write("Hello, Word") // irá exibir e mensagem diretamente no navegador
```
## Variáveis
### var(forma mais antiga) pode ser alterada
```js
var idade = 30// declarou o valor 30
idade = 31 // mudou o valor para 31
console.log(idade) // o valor vai sair 31
```
### let(forma mais moderna) pode ser alterada
```js
let idade = 30// declarou o valor 30
idade = 31 // mudou o valor para 31
console.log(idade) // o valor vai sair 31
```
### const(constante) não pode ser alterada
```js
const idade = 30// declarou o valor 30
console.log(idade) // o valor vai sair 30
```
## Tipos Primitivos
### String(para reprensentar textos) pode usar aspas simples,aspas duplas,crase
```js
let aspasimples = "maria"
let aspasduplas = 'maria'
let crase = `maria`
```
### Number(Usada para representar Números)
```js
let n1 = 2
let n2 = 5.3
```
### Boolean(Usado para representar um valor verdadeiro ou falso(usado muito em condições ou em loops)
```js
let estativo = true
let usuarioautenticado = false
```
## Convertendo de String Para numero
#### Para converter uma String em um número inteiro ou decimal usamos o ParseInt() ou ParseFloat()
### parseInt() para Inteiros
```js
let str = "123.45"
let num = parseInt(str)
console.log(num)//123
```
### parseFloat() para decimal
```js
let str = "123.45"
let num = parseFloat(str)
console.log(num)//123.45
```
## Concatenação
### E usado para unir string, outros valores podemos usar: +(sinal da soma),${}(template String),Concat

### + (sinal de soma)
```js
const nome = "lucas"
const sobrenome = " Vasconcelos"
console.log(nome + sobrenome)
```
### Templete String ${}
```js
const nome = "lucas"
const sobrenome = "Vasconcelos"
console,log(`Olá ${nome} esse e seu nome,seu sobrenome e ${sobrenome}`) // usamos a crase no Templete String
```
### Concat()
```js
const nome = "lucas "
const sobrenome = "Vasconcelos"
const competo = nome.concat(sobrenome)
console.log(completo)// vai sair lucas Vasconcelos
```
## Operadores
#### são símbolos especiais que indicam para o computador realizar uma determinada operação,existem as Aritméticos,Relacionais,Lógicos,Atribuição
## Aritméticas  São representados por +,-,/,*,%
### + soma dos valores
```js
const n1 = 9
const n2 = 10
console.log(n1 + n2)// vai retorna 19
```
### - subtração dos valores
```js
const n1 = 9
const n2 = 10
console.log(n1 - n2)// vai retorna 1
```
### / dvisão dos valores
```js
const n1 = 10
const n2 = 2
console.log(n1 / n2)// vai retorna 5
```
### * multiplicação dos valores
```js
const n1 = 10
const n2 = 2
console.log(n1 * n2)// vai retorna 20
```

### % resto de uma divisão
```js
let numero = 13
let resto = numero % 2
console.log(resto) // 1
```
## Relacionados são representados por >,<,>=,<=,==,!=,
### > maior que
```js
const n1 = 7
const n2 = 4
console.log(n1 > n2) // retorna true que o valor de n1 e maior que o valor de n2

```
### < menor que
```js
const n1 = 7
const n2 = 4
console.log(n1 < n2) // retorna false que o valor de n1 e maior que o valor de n2

```
### >= maior ou igual que
```js
const n1 = 7
const n2 = 4
console.log(n1 >= n2) // retorna true que o valor de n1 e maior que o valor de n2, ou se o valor fosse igual iria retonar o valor true também

```
### <= menor ou igual que
```js
const n1 = 7
const n2 = 4
console.log(n1 <= n2) // retorna false que já que o 7 e maior que 4, se fosse igual também retornaria igual
 
```
### == igual
```js
const nome = prompt("Digite seu nome")
console.log(nome == "lucas") // se o usuario digitar lucas vai aparecer true, se não vai parecer false
```
### !=  diferente
```js
const nome = prompt("Digite seu nome")
console.log(nome != "lucas") // se o usuario digitar lucas vai aparecer false, se não vai parecer true
```
## lógicos ||,&&
###  ||- se operador tem ns. tentativa
```js
const nome = prompt("Digite seu nome")
console.log(nome == "lucas" || nome == "dmd") // seu o nome digitado for lucas ou dmd vai retornar true,se não false
```
###  &&-  E lógico
```js
let numero = 10;
if (numero > 5 && numero < 15) {
  console.log("O número está entre 5 e 15");
}
```
## Dom(document object Moldel)
### É uma representação de uma página HTML e de todos os seus conteúdos, Ele se assemelha a uma árvore cujas <br> galhos são no, onde cada tag e conteúdo geram uns nó, tudo em página HTML é um nó na árvore do Dom, de onde podem Surgir ainda outros nós filhos.
   <img src="https://hermes.dio.me/articles/cover/315351e5-1c6e-4bad-8690-34a014fc88ec.png" height="460px" weight="120px">
   
## Composição do DOM
### Nó Documento: O Próprio documento HTML.
### Nó Elemento: Todas as tags existentes dentro do arquivo HTML e que se transforman em elemntos dentro da árvore DOM.
### Nó texto: o conteúdo de texto esistente dentro das tags.
### Nó Atributo: Todos os Atributos existentes dentro das tags em especifico Ex: href,id,class,dentro outros.

## Importância do DOM
### para realizarmos alterações na esttrutura do HTML, nos seus estilos,modificar conteúdos e adicionar os mais diversos eventos
## Métodos de Manipulação do DOM
## getElementById()
### Retorna o conteúdo do elemento HTML que estiver com o nome de Id informado,os Ids devem ser nomes únicos.
```js
let input = document.getElementById("text-input")
```
## getElementsByTagName()
### Retorna uma coleção de todas os elementos que contenham o nome da tag informada,caso tenha mais de uma tag igual vai pelo[ ] que começa pelo 0
```js
const m = document.getElementsBytagName("p")[0]
```
## querySelector()
### Retorna qualquer Elemento do DOM, como Classes,tags e ID's, você apenas precisa deixar explicativo se está chamando uma classe, um ID ou uma tag. Id = #, classes = .,Sim as classes usam pontos
```js
let getInputid = document.querySelector("#textinput")
let getInputclass = document.querySelector(".text-input")
let getInputtag = document.querySelector("input")
```
## getElementByClass()
### esse método nos permite selecionar elementos do documento incluidos dentro do atributo class,recebe um único argumento de String, que pode conter vários indentificadores separados por espaços

## Modificação do HTML pelo JAVASCRIPT
## Innertext
### Modifica o conteúdo do texto de um elemento
```js
p.innertext = "novo texto"
```
## InnerHtml
### Modifica o contéudo HTML intertno de um elemento
```js
p.innerthtml="<b>texto em negrito</b>"
```
## Modificação do CSS pelo JavaSCript
## Style
### Utilizada para Selecionar ou Modificar uma Regra de Estilização
```js
document.getElementById("myh1").style.color="red"
```
## Eventos no JavaScript
### Eventos são basicamente um conjunto de açõoes que são realizadas em um determinado elemento da página web,seja ele um texto, uma div, por EXemplo, eventos podem ser algo que o brawser faz,ou que o usuário faça por Exemplo:
### - A Finalização de carregamento de uma página HTML
### - Um Campo Input que foi Prenchido pelo Usuário
### - Um Botão que Foi Clicado


| OndClick|Disparado quando o Click Duplo |
|---|---|
| Onmouseover |Disparado Quando o Mouse está sobre| 
| onmousemove |Disparado quando o mouse é movido | 
| onmouseout  |Disparado quando o mouse é movido para fora do elemento | 
| onmousedown |Disparado quando o Clique do botão for Pressionado | 
| onkeypress |Disparado quando a tecla e pressionada e seta sobre um elemento| 
| onkeyPress |Disparado quando o mouse é movido | 
