# 1010 Cálculo Simples

Neste problema, deve-se ler o código de uma peça 1, o número de peças 1, o valor unitário de cada peça 1, o código de uma peça 2, o número de peças 2 e o valor unitário de cada peça 2. Após, calcule e mostre o valor a ser pago.

## Entrada

O arquivo de entrada contém duas linhas de dados. Em cada linha haverá 3 valores, respectivamente dois inteiros e um valor com 2 casas decimais.

## Saída

A saída deverá ser uma mensagem conforme o exemplo fornecido abaixo, lembrando de deixar um espaço após os dois pontos e um espaço após o "R$". O valor deverá ser apresentado com 2 casas após o ponto.

## Exemplo de Entrada & Saída

| Entrada                    | Saída                   |
| -------------------------- | ----------------------- |
| 12 1 5.30 <br> 16 2 5.10   | VALOR A PAGAR: R$ 15.50 |
| 13 2 15.30 <br> 161 4 5.20 | VALOR A PAGAR: R$ 51.40 |
| 1 1 15.10 <br> 2 1 15.10   | VALOR A PAGAR: R$ 30.20 |

## Código Fonte

```javascript
var input = require("fs").readFileSync("/dev/stdin", "utf8");
var lines = input.trim().split("\n");

function Calculation(quantity, value) {
  return quantity * value;
}

function Sum(number, index = 0) {
  if (index === number.length) {
    return 0;
  }
  return number[index] + Sum(number, index + 1);
}

let soma = [];

for (let i = 0; i < lines.length; i++) {
  let [id, quantity, value] = lines[i].split(" ").map((v) => parseFloat(v));

  soma.push(Calculation(quantity, value));
}

console.log("VALOR A PAGAR: R$", Sum(soma).toFixed(2));
```

## Submissão

```yaml
Problema: 1010 - Cálculo Simples
Resposta: Accepted
Linguagem: JavaScript
Tempo: 0.060s
Tamanho: 580 Bytes
Memória: -
Submissão: 13/08/2025 21:05:46
```
