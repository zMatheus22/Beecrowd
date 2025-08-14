# 1007 Diferença

Leia quatro valores inteiros A, B, C e D. A seguir, calcule e mostre a diferença do produto de A e B pelo produto de C e D segundo a fórmula: DIFERENCA = (A _ B - C _ D).

## Entrada

O arquivo de entrada contém 4 valores inteiros.

## Saída

Imprima a mensagem **DIFERENCA** com todas as letras maiúsculas, conforme exemplo abaixo, com um espaço em branco antes e depois da igualdade.

## Exemplo de Entrada & Saída

| Entrada                 | Saída           |
| ----------------------- | --------------- |
| 5 <br> 6 <br> 7 <br> 8  | DIFERENCA = -26 |
| 0 <br> 0 <br> 7 <br> 8  | DIFERENCA = -56 |
| 5 <br> 6 <br> -7 <br> 8 | DIFERENCA = 86  |

## Código Fonte

```javascript
var input = require("fs").readFileSync("/dev/stdin", "utf8");
var lines = input.split("\n");

function Diferenca(A, B, C, D) {
  return A * B - C * D;
}

const x = parseInt(lines[0]);
const y = parseInt(lines[1]);
const z = parseInt(lines[2]);
const w = parseInt(lines[3]);

console.log("DIFERENCA =", Diferenca(x, y, z, w));
```

## Submissão

```yaml
Problema: 1007 - Diferença
Resposta: Accepted
Linguagem: JavaScript
Tempo: 0.300s
Tamanho: 341 Bytes
Memória: -
Submissão: 13/08/2025 20:03:45
```
