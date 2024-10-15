# Caderno virtual - Lógica da Programação e Algoritmos




## JavaScript
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/99/Unofficial_JavaScript_logo_2.svg/1200px-Unofficial_JavaScript_logo_2.svg.png" height="50" width="50">


## Exibir Mensagens
```js
//console.log() exibe mensagem no console do navegador
console.log("Hello, Word")// irá exibir Hello, Word no console do navegador
```
```js
//document.write() exibe a mensagem diretamenta na página(usado junto com html)
document.write("Hello, Word") // irá exibir e mensagem diretamente no navegador)
```
## Variáveis
```js

//var(forma mais antiga) pode ser alterada
var idade = 30// declarou o valor 30
idade = 31 // mudou o valor para 31
console.log(idade) // o valor vai sair 31
```
```js

//let(forma mais moderna) pode ser alterada
let idade = 30// declarou o valor 30
idade = 31 // mudou o valor para 31
console.log(idade) // o valor vai sair 31
```
```js

//const(constante) não pode ser alterada
consty idade = 30// declarou o valor 30
console.log(idade) // o valor vai sair 30
```
## Tipos Primitivos
```js
//String(para reprensentar textos) pode usar aspas simples,aspas duplas,crase
let aspasimples = "maria"
let aspasduplas = 'maria'
let crase = `maria`
```
```js
//Number(Usada para representar Números)
let n1 = 2
let n2 = 5.3
```
```js
//Boolean(Usado para representar um valor verdadeiro ou falso(usado muito em condições ou em loops)
let estativo = true
let usuarioautenticado = false
```
## Convertendo de String Para numero
#### Para converter uma String em um número inteiro ou decimal usamos o ParseInt() ou ParseFloat()

### ParseInt() para Inteiros
```js
let str = "123.45"
let num = ParseInt(str)
console.log(num)//123
```
### ParseFloat() para decimal
```js
let srt = "123.45"
let num = ParseFloat(str)
console.log(num)//123.45
```
## Concatenação
#### E usado para unir string, outros valores podemos usar: +(sinal da soma),${}(template String),Concat

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
## + soma dos valores
```js
const n1 = 9
const n2 = 10
console.log(n1 + n2)// vai retorna 19
```
## - subtração dos valores
```js
const n1 = 9
const n2 = 10
console.log(n1 - n2)// vai retorna 1
```
## / dvisão dos valores
```js
const n1 = 10
const n2 = 2
console.log(n1 / n2)// vai retorna 5
```
## * multiplicação dos valores
```js
const n1 = 10
const n2 = 2
console.log(n1 * n2)// vai retorna 20
```

## % resto de uma divisão
```js
let numero = 13
let resto = numero % 2
 console.log(resto) // 1
```




