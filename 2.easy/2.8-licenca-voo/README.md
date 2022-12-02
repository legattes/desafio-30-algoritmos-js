Strings
Classes
Datas
14. Licença de Voo
Para pilotar uma nave de pequeno porte em qualquer planeta da Federação é preciso possuir uma licença de voo.
O código usado na licença de voo é criado a partir de informações de seu dono, como nome e data de nascimento.
Foi solicitado que você crie um método para gerar a licença de voo de uma determinada pessoa para ser integrado aos sistemas da Federação. É obrigatório fazer isso utilizando uma classe.

# Desafio
Escreva uma classe que contenha um método para gerar uma licença de voo e os seguintes atributos:
Nome
Sobrenome
Data de Nascimento
Licença de Voo (que deve iniciar sempre como falso)
Além disso a classe deve possuir um método para criar uma licença caso a pessoa ainda não possua uma. A licença deve ser uma string seguindo o seguinte padrão:
Os primeiros cinco caracteres do sobrenome em letras maiúsculas (completado com 9's caso possua menos de cinco)
O 6º caractere é um traço (-)
0 7° caractere é o algarismo da década (penúltimo) do ano de nascimento
0 8° e 9º caracteres são o mês de nascimento
0 10° caractere é o algarismo do ano (último) do ano de nascimento
O 11° caractere é um ponto (.)
0 12° caractere é a primeira letra do primeiro nome (minúscula)

# Testes
- Pilot {
    firstName: "John",
    lastName: "Doe",
    birthday: 1977-05-25T03:00:00.000Z,
    flyingLicense: "DOE99-7057.j"
}
- Pilot {
    firstName: "Hal",
    lastName: "Jordan",
    birthday: 1995-09-02T03:00:00.000Z,
    flyingLicense: "JORDA-9095.h"
}
- Pilot {
    lastName: "Danvers",
    firstName: "Carol",
    birthday: 1968-08-17T03:00:00.000Z,
    flyingLicense: "DANVE-6088.c"
}
- Pilot {
    firstName: "Poe",
    lastName: "Dameron",
    birthday: 1979-03-09T03:00:00.000Z,
    flyingLicense: "DAMER-7039.p"
}
