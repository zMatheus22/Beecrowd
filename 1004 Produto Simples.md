# Produto Simples

Leia dois valores inteiros. A seguir, calcule o produto entre estes dois valores e atribua esta operação à variável PROD. A seguir mostre a variável PROD com mensagem correspondente.

## Entrada

O arquivo de entrada contém 2 valores inteiros.

## Saída

Imprima a mensagem "PROD" e a variável PROD conforme exemplo abaixo, com um espaço em branco antes e depois da igualdade. Não esqueça de imprimir o fim de linha após o produto, caso contrário seu programa apresentará a mensagem: “Presentation Error”.

## Exemplo de Entrada & Saída

| Entrada     | Saída       |
| ----------- | ----------- |
| 3 <br> 9    | PROD = 27   |
| -30 <br> 10 | PROD = -300 |
| 0 <br> 9    | PROD = 0    |

## Código Fonte

```javascript
var input = require("fs").readFileSync("/dev/stdin", "utf8");
var lines = input.split("\n");

function Multiplicacao(a, b) {
  return a * b;
}

const x = lines[0];
const y = lines[1];

console.log("PROD = " + Multiplicacao(x, y));
```

## Submissão

```yaml
Problema: 1004 - Produto Simples
Resposta: Accepted
Linguagem: JavaScript
Tempo: 0.086s
Tamanho: 242 Bytes
Memória: -
Submissão: 12/08/2025 22:36:59
```
