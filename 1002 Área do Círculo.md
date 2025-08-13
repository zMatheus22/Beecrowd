# Área do Círculo

A fórmula para calcular a área de uma circunferência é: `area = π . raio²`. Considerando para este problema que **π = 3.14159**:

- Efetue o cálculo da área, elevando o valor de **raio** ao quadrado e multiplicando por **π**.

## Entrada

A entrada contém um valor de ponto flutuante (dupla precisão), no caso, a variável raio.

## Saída

Apresentar a mensagem "A=" seguido pelo valor da variável area, conforme exemplo abaixo, com 4 casas após o ponto decimal. Utilize variáveis de dupla precisão (double). Como todos os problemas, não esqueça de imprimir o fim de linha após o resultado, caso contrário, você receberá "Presentation Error".

## Exemplo de Entrada & Saída

| Entrada | Saída        |
| ------- | ------------ |
| 2.00    | A=12.5664    |
| 100.64  | A=31819.3103 |
| 150.00  | A=70685.7750 |

## Código Fonte

```javascript
var input = require("fs").readFileSync("/dev/stdin", "utf8");
var lines = input.split("\n");

const raio = parseFloat(lines[0]);
const pi = 3.14159;
const area = pi * raio * raio;

console.log("A=" + area.toFixed(4));
```

## Submissão

```yaml
Problema: 1002 - Área do Círculo
Resposta: Accepted
Linguagem: JavaScript
Tempo: 0.603s
Tamanho: 224 Bytes
Memória: -
Submissão: 12/08/2025 22:23:00
```
