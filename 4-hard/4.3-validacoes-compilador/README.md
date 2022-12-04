# Assuntos
- Strings

# 25. Validações do Compilador
Você e sua equipe estão trabalhando em um compilador que deverá converter o código escrito em uma linguagem moderna para uma outra linguagem mais antiga que é utilizada pelo sistema principal da sua nave.
Uma das tarefas da qual você ficou encarregado foi a de validar o uso de parêntesis, colchetes e chaves no código.
Para que sejam válidos os agrupamentos deve ser abertos e fechados corretamente.

# Desafio
Escreva uma função que recebe uma string, verifica se ela possui uma distribuição válida de parêntesis, colchetes e chaves, e retorna true ou false baseada nessa verificação.
A função deve ser capaz de funcionar com qualquer string independente do conteúdo que acompanha os parêntesis, colchetes e chaves.

# Testes
- Entrada: ("((((([(]))))))")
  - Saída: false
- Entrada: ('{(){([]){[]}()()()()[]}(){(())}(())}")
  - Saída: true
- Entrada: Utilize o código de um desafio que você tenha feito até agora.
  - Saída: true
- Entrada: Utilize o código de um desafio que você tenha feito até agora com um erro proposital nos parêntesis.
  - Saída: false