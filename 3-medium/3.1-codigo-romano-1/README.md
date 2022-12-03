# Assuntos
- Matemática
- Manipulação de Tipos

# 15. Código Romano I
Em uma missão por regiões não mapeadas pela Federação sua equipe encontrou um povoado que utilizava um sistema numérico muito parecido com o romano.
Você foi encarregado de implementar um tradutor capaz de converter qualquer número (em formato de texto) para o seu inteiro decimal correspondente.

# Desafio
Escreva uma função que recebe uma string de algarismos romanos e seja capaz de traduzir seu conteúdo retornando o inteiro decimal correspondente.
Os algarismos romanos são:
- I: 1
- V: 5
- X: 10
- L: 50
- C: 100
- D: 500
- M: 1000
Os outros números são formados a partir de dois tipos de notação, a padrão e a subtrativa.
Notação Padrão: I, II e III (1, 2 e 3), VI, VII e VIII (6, 7 e 8), X, XX e XXX (10, 20 e 30), etc.
Notação Subtrativa: IV (1-5 = 4), IX (1-10 = 9), XLIX (10-50+1-10 = 49), XC (10-100 = 90), CMXCIX (100-1000+10-100+1-10 = 999)

# Testes
- Entrada: ('XLVII')
  - Saída: 47
- Entrada: ('CDXXXVIII)
  - Saída: 438
- Entrada: ('CMIX')
  - Saída: 909
- Entrada: ('MMMCMXCIX')
  - Saída: 3999