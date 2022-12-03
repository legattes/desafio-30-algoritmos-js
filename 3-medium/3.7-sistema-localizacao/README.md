# Assuntos
- Matemática
- Classes
- Estruturas Básicas

# 21. Sistema de Localização
A estação espacial Olympus, que está nas etapas finais de sua construção, possui um sistema de rastreamento que deve ser capaz de localizar coordenadas próximas a partir da sua própria posição.
Para isso, você foi incumbido da tarefa de construir parte desse sistema.
Você deve construir uma classe capaz de armazenar um ponto de 3 coordenadas numéricas e também detectar o setor em que elas se encontram.
Além disso, também deve ser capaz de calcular a distância entre o ponto e a estação espacial.

# Desafio
Escreva uma classe que seja capaz de armazenar 3 coordenadas, determinar o setor em que se encontram suas coordenadas e sua distância em relação à estação espacial (coordenada [0, 0, 0]).
Distribuição dos setores:
- Alfa: [positivo, positivo, positivo]
- Beta: [positivo, positivo, negativo]
- Gama: [positivo, negativo, positivo]
- Delta: [positivo, negativo, negativo]
- Épsilon: [negativo, positivo, positivo]
- Zeta: [negativo, positivo, negativo]
- Sigma: [negativo, negativo, positivo]
- Ômega: [negativo, negativo, negativo]

Considere 0 como positivo para garantir que um ponto estará apenas em um único setor.

# Testes
- Entrada: ([37, 42, 15])
  - Saída setor: Alfa
  - Saída distância: 57.94825277780168
- Entrada: ([144, 49, 0])
  - Saída setor: Alfa
  - Saída distância; 152.10851389715174
- Entrada: ([-37, 0, 0])
  - Saída setor: Épsilon
  - Saída distância: 37
- Entrada: ([-19, -80, -32])
  - Saída setor: Delta
  - Saída distância: 88.23264701911646