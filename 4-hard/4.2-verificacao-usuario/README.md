# Assuntos
- Strings
- RegEx

# 24. Verificação de Usuário
Em uma nave de grande porte existem muitos terminais de acesso ao sistema principal, e para se conectar através deles um membro da tripulação deve utilizar seu nome de usuário, senha e verificação biométrica.
O nome de usuário deve ser validado segundo algumas regras antes que possa ser cadastrado.
Sua tarefa atual é construir um mecanismo de validação de nomes de usuário para ser utilizado pelo sistema de cadastro.

# Desafio
Escreva uma função que recebe uma string e verifica se ela atende aos seguintes requisitos:
- Deve conter entre 4 e 32 caracteres.
- Deve conter apenas letras (sem acentos), números ou_
- Deve começar com uma letra
- Não pode terminar com _
- Deve conter pelo menos um de cada tipo de caractere (letra, número e underscore)
- Deve ser único
  - Obs.: Para isso você pode utilizar qualquer meio que achar válido para simular um banco de dados, como um array contendo vários nomes fictícios para comparação, por exemplo. Caso atenda, retorne true, caso não atenda retorne false.

# Testes
- Usuários Já Registrados: ['erick_14', 'pam_ls2', 'VICTOR_99A']

- Entrada: ('52alfred')
  - Saída: false
- Entrada: ('erick_14')
  - Saída: false
- Entrada: ('josh_g15')
  - Saída: true
- Entrada: ('hugo123_')
  - Saída: false
- Entrada: ('k_9')
  - Saída: false