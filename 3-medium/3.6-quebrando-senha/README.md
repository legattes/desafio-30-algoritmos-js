# Assuntos
- Recursão
- Arrays

# 20. Quebrando a Senha
Em uma missão no planeta Darnas a equipe de reconhecimento encontrou diversos dispositivos que parecem ter informações cruciais para a missão, porém os dispositivos estão bloqueados por senhas.
Você e seu colega estão criando um procedimento para descobrir as senhas utilizando força bruta.
Você ficou encarregado de criar a função que irá calcular todas as senhas possíveis a partir da lista de caracteres que a compõe.

# Desafio
Escreva uma função que receba um array de opções e retorne um array bidimensional de todas as senhas. possíveis utilizando todos os elementos passados. Faça isso utilizando recursão.

# Testes
- Entrada: (["X", "s", "-", "#"])
  - Saída: [
        ["X", "s", "-", "#"], ["s", "X", "-", "#"],
        ["s","-", "X", "#"], ["s", "", "#", "X"],
        ["X", "", "s", "#", ["-", "X", "s", "#"],
        ["-", "s", "X", "#"], ["-", "s", "#", "X"],
        ["X", "-", "#", "s"], ["-", "X", "#", "s"],
        ["-", "#", "X", "s"], ["-", "#", "s", "X"],
        ["X", "s", "#", "-"], ["s", "X", "#", "-"],
        ["s", "#", "X", "-"], ["s", "#", "-", "X"],
        ["X", "#", "s", "-"], ["#", "X", "s", "-"],
        ["#", "s", "X", "-"], ["#", "s", "-", "X"],
        ["X", "#", "-", "s"], ["#", "X", "-", "s"],
        ["#", "-", "X", "s"], ["#", "", "s", "X"]
    ]
- Entrada: (["1", "2", "3"])
  - Saída: [["1", "2", "3"], ["2", "1", "3"], ["2", "3", "1"], ["1", "3", "2"], ["3", "1", "2"], ["3", "2", "1"]]
- Entrada: ([])
  - Saída: [[]]