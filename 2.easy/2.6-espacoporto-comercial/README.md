# Assuntos
- Matemática

# 12. Espaçoporto Comercial
A sua nave está de passagem por um planeta que usa como dinheiro as moedas de créditos.
Existem moedas de 1, 5, 10, 25, 100 e 500 créditos.
Para conseguir um favor de um comerciante local você irá ajudá-lo a automatizar o processo de contagem das moedas através de um programa que calcula quantas de cada moeda ele irá precisar para chegar a um valor determinado.

# Desafio
Escreva uma função que receba um valor inteiro e retorne a quantidade de cada moeda para se chegar ao valor.
Deve-se sempre priorizar as moedas de maior valor (o máximo possível de moedas de 500, depois o máximo possível de moedas de 100, etc).

# Testes
- Entrada: 478
  - Saída: {"1": 3, "5": 0, "10": 0, "25": 3, "100": 4, "500": 0}
- Entrada: 384
  - Saída: {"1": 4, "5": 1, "10": 0, "25": 3, "100": 3, "500": 0}
- Entrada: 5412
  - Saída: {"1": 2, "5": 0, "10": 1, "25": 0, "100": 4, "500": 10 }
- Entrada: 50
  - Saída: { "1": 0, "5": 0, "10": 0, "25": 2, "100": 0, "500": 0}