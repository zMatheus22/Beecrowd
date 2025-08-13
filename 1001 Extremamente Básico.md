# Extremamente Básico

Leia 2 valores inteiros e armazene-os nas variáveis A e B. Efetue a soma de A e B atribuindo o seu resultado na variável X. Imprima X conforme exemplo apresentado abaixo. Não apresente mensagem alguma além daquilo que está sendo especificado e não esqueça de imprimir o fim de linha após o resultado, caso contrário, você receberá "Presentation Error".

## Entrada

A entrada contém 2 valores inteiros.

## Saída

Imprima a mensagem "X = " (letra X maiúscula) seguido pelo valor da variável X e pelo final de linha. Cuide para que tenha um espaço antes e depois do sinal de igualdade, conforme o exemplo abaixo.

## Exemplo de Entrada & Saída

| Entrada    | Saída  |
| ---------- | ------ |
| 10 <br> 9  | X = 19 |
| -10 <br> 4 | X = -6 |
| 15 <br> -7 | X = 8  |

## Código Fonte

```javascript
var input = require("fs").readFileSync("/dev/stdin", "utf8");
var lines = input.split("\n");

const A = parseInt(lines[0]);
const B = parseInt(lines[1]);

const soma = A + B;

console.log("X = " + soma);
```

## Submissão

```yaml
Problema: 1001 - Extremamente Básico
Resposta: Accepted
Linguagem: JavaScript
Tempo: 0.481s
Tamanho: 214 Bytes
Memória: -
Submissão: 12/08/2025 22:02:46
```
