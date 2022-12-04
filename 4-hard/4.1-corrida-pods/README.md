# Assuntos
- Strings
- Arrays

# 23. Corrida de Pods
Corridas de pods são muito rápidas e perigosas, mas seres de todos os planetas adoram.
Para acompanhar a classificação durante a corrida foi requisitado que você construa um programa que atualize a lista com a posição de todos os corredores a medida que eles vão ultrapassando uns aos outros ou sendo eliminados da corrida.

# Desafio
Escreva um programa que receba uma lista de classificação de nomes e uma string no formato "Nome +n" (ou -n), onde n é a quantidade de posições para subir ou descer na classificação, e retorne essa mesma lista com a classificação atualizada.
A função também deve ser capaz de receber "Nome ELIMINATE", nesse caso o participante deve ser jogado para o fim da lista e deve ser acrescentado um " ELIMINATED" ao seu nome, indicando que ele foi eliminado.
Os participantes eliminados não podem ter nenhum corredor não eliminado atrás deles na lista.
Assuma que sempre receberá uma entrada válida no formato "Corredor AÇÃO".

# Testes
- Classificação Inicial: "Alfa", "Beta", "Gama" e "Delta"

- Entrada: ("Beta +1")
  - Classificação: "Beta", "Alfa", "Gama" e "Delta"
- Entrada: ("Gama -1")
  - Classificação: "Beta", "Alfa", "Delta" e "Gama"
- Entrada: ("Delta ELIMINATE")
  - Classificação: "Beta", "Alfa", "Gama" e "Delta ELIMINATED"
- Entrada: ("Gama +2")
  - Classificação: "Gama", "Beta", "Alfa" e "Delta ELIMINATED"