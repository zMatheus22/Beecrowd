# Soma Simples

Leia dois valores inteiros, no caso para variáveis A e B. A seguir, calcule a soma entre elas e atribua à variável SOMA. A seguir escrever o valor desta variável.

## Entrada

O arquivo de entrada contém 2 valores inteiros.

## Saída

Imprima a mensagem "SOMA" com todas as letras maiúsculas, com um espaço em branco antes e depois da igualdade seguido pelo valor correspondente à soma de A e B. Como todos os problemas, não esqueça de imprimir o fim de linha após o resultado, caso contrário, você receberá "Presentation Error".

## Exemplo de Entrada & Saída

| Entrada     | Saída      |
| ----------- | ---------- |
| 30 <br> 10  | SOMA = 40  |
| -30 <br> 10 | SOMA = -20 |
| 0 <br> 0    | SOMA = 0   |

## Código Fonte

```javascript
var input = require("fs").readFileSync("/dev/stdin", "utf8");
var lines = input.split("\n");

function Soma(a, b) {
  return a + b;
}

const x = parseInt(lines[0]);
const y = parseInt(lines[1]);

console.log("SOMA = " + Soma(x, y));
```

## Submissão

```yaml
Problema: 1003 - Soma Simples
Resposta: Accepted
Linguagem: JavaScript
Tempo: 0.098s
Tamanho: 247 Bytes
Memória: -
Submissão: 12/08/2025 22:30:33
```
