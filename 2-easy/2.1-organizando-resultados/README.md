# Assuntos
- Arrays

# 7. Organizando Resultados
O sistema interno da nave realiza periodicamente uma verificação de seus principals componentes para checar sua integridade.
Os varios resultados dessa verificação são emitidos em formato de listas de referências numéricas desorganizadas.
Para otimizar isso você deve criar um procedimento que seja capaz de organizar todas as listas de números em uma única lista ordenada.

# Desafio
Escreva uma função que recebe um array bidimensional e inteiros e retorna um unico array contendo todos os números em ordem ascendente.

# Testes
- Entrada: [[1, 5, 3], [6, 19, 11], [47, 128, 5], [1, 93, 57, 42, 103]]
  - Saída: [1, 1, 3, 5, 5, 6, 11, 19, 42, 47, 57, 93, 103, 128]
- Entrada: [[1, 3], [4, 8], [7, 5], [2, 6]]
  - Saída: [1, 2, 3, 4, 5, 6, 7, 8]
- Entrada: [[], [], [], []]
  - Saída: []
- Entrada: [[100, 50], [60, 100], [20, 100, 70], [10, 40, 80, 90]]
  - Saída: [10, 20, 40, 50, 60, 70, 80, 90, 100, 100, 100]