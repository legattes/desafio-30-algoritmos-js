# Assuntos
- Classes
- Matemática

# 18. Módulo de Treinamento
Na colônia estabelecida no planeta primitivo Romulus está sendo criada uma escola a fim de fornecer educação básica para os colonos.
Para auxiliar durante as aulas de matemática, foi solicitado que uma equipe construísse um programa de computador capaz de explicar e resolver diversos tipos de problemas e conceitos.
Como parte da equipe, você foi encarregado de construir o módulo que trata de equações até o segundo grau, portanto precisará construir um programa capaz de resolver equações e descrever os passos da resolução.
É obrigatório o uso de classes.

# Desafio
Escreva uma classe Equation que seja capaz de lidar com uma equações até o segundo grau.
Os objetos podem ser instanciados com valores padrões para a = 0, b = 0 e c = 0.
Ela deve ter um método para retornar suas raízes na forma de um array vazio, de um ou de dois elementos.
O método também deve descrever os passos para a resolução da equação.
Se a, b e c forem todos iguais a 0 ela não deve calcular as raízes e deve retornar uma mensagem de erro.

# Testes
- Entrada: (0, 2, 6)
  - Saída:
    - 1. 2x + 6 = 0
    - 2. 2x = -6
    - 3. x = -6/2
    - 4. x = -3
    - [-3]
- Entrada: ()
  - Saída: "Erro! Nenhum parâmetro informado."
- Entrada: (0, 0, 5)
  - Saída:
    - 1. Parâmetros insuficientes.
    - Nenhuma raiz real.
    - []
- Entrada: (1, -4, -5)
  - Saída:
    - 1. A = -4² - 4*1*-5
    - 2. A = 36
    - 3. x' = (-(-4)+ √36) / 2*1
    - 4. x'' = (-(-4) - √36) / 2*1
    - 5. x' = 4+ √36/2
    - 6. x'' = 4 - √36/2
    - 7. x = 4 + 6/2
    - 8. x'' = 4 - 6/2
    - 9. x' = 5
    - 10. x'' = -1
    - [5, -1]