# 1009 Salário com Bônus

Faça um programa que leia o nome de um vendedor, o seu salário fixo e o total de vendas efetuadas por ele no mês (em dinheiro). Sabendo que este vendedor ganha 15% de comissão sobre suas vendas efetuadas, informar o total a receber no final do mês, com duas casas decimais.

## Entrada

O arquivo de entrada contém um texto (primeiro nome do vendedor) e 2 valores de dupla precisão (double) com duas casas decimais, representando o salário fixo do vendedor e montante total das vendas efetuadas por este vendedor, respectivamente.

## Saída

Imprima o total que o funcionário deverá receber, conforme exemplo fornecido.

## Exemplo de Entrada & Saída

| Entrada                             | Saída              |
| ----------------------------------- | ------------------ |
| JOAO <br> 500.00 <br> 1230.30       | TOTAL = R$ 684.54  |
| PEDRO <br> 700.00 <br> 0.00         | TOTAL = R$ 700.00  |
| MANGOJATA <br> 1700.00 <br> 1230.50 | TOTAL = R$ 1884.58 |

## Código Fonte

```javascript
var input = require("fs").readFileSync("/dev/stdin", "utf8");
var lines = input.split("\n");

function SalaryWithCommission(salary, valueCommission, percentCommission) {
  return salary + valueCommission * (percentCommission / 100);
}

const name = lines[0];
const salary = parseFloat(lines[1]);
const commission = parseFloat(lines[2]);
const percent = 15;

console.log(
  "TOTAL = R$",
  SalaryWithCommission(salary, commission, percent).toFixed(2)
);
```

## Submissão

```yaml
Problema: 1009 - Salário com Bônus
Resposta: Accepted
Linguagem: JavaScript
Tempo: 0.328s
Tamanho: 460 Bytes
Memória: -
Submissão: 13/08/2025 20:24:37
```
