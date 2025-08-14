# 1008 Salário

Escreva um programa que leia o número de um funcionário, seu número de horas trabalhadas, o valor que recebe por hora e calcula o salário desse funcionário. A seguir, mostre o número e o salário do funcionário, com duas casas decimais.

## Entrada

O arquivo de entrada contém 2 números inteiros e 1 número com duas casas decimais, representando o número, quantidade de horas trabalhadas e o valor que o funcionário recebe por hora trabalhada, respectivamente.

## Saída

Imprima o número e o salário do funcionário, conforme exemplo fornecido, com um espaço em branco antes e depois da igualdade. No caso do salário, também deve haver um espaço em branco após o $.

## Exemplo de Entrada & Saída

| Entrada               | Saída                               |
| --------------------- | ----------------------------------- |
| 25 <br> 100 <br> 5.50 | NUMBER = 25 <br> SALARY = U$ 550.00 |
| 1 <br> 200 <br> 20.50 | NUMBER = 1 <br> SALARY = U$ 4100.00 |
| 6 <br> 145 <br> 15.55 | NUMBER = 6 <br> SALARY = U$ 2254.75 |

## Código Fonte

```javascript
var input = require("fs").readFileSync("/dev/stdin", "utf8");
var lines = input.split("\n");

function Salary(hour, value) {
  return value * hour;
}

const id_employee = parseInt(lines[0]);
const hour_employee = parseFloat(lines[1]);
const value_employee = parseFloat(lines[2]);

console.log("NUMBER =", id_employee);
console.log("SALARY = U$", Salary(hour_employee, value_employee).toFixed(2));
```

## Submissão

```yaml
Problema: 1008 - Salário
Resposta: Accepted
Linguagem: JavaScript
Tempo: 0.379s
Tamanho: 411 Bytes
Memória: -
Submissão: 13/08/2025 20:12:41
```
