# Assuntos
- Classes
- Objetos
- Arrays
- Matemática

# 28. Hora de Jogar
Há exatamente 100 anos, quando a exploração de novos planetas ainda era algo reservado apenas para as ficções-científicas, um RPG de mesa muito popular te permitia viver aventuras em outros planetas como um explorador do espaço.
Agora, para comemorar essa data especial uma equipe está criando uma versão digital deste mesmo jogo e você foi designado para cooperar com ela no desenvolvimento.
Sua tarefa no momento é criar, de acordo com uma lista de requisitos, uma classe que representa um explorador e que será incluída no jogo final.
É obrigatório o uso de classes.

# Desafio
Escreva uma classe que calcula e mantém informações sobre exploradores, como seus nível e habilidades. Ela precisará obedecer aos seguintes requisitos:
Sobre o nível:
- Um explorador começa no nível 1 e pode evoluir até o nível 99.
- O explorador não deve subir de nível após o nível 99, mas pode acumular pontos de experiência.
- Para subir de nível o explorador deve acumular 100 pontos + 10 pontos * o seu nível atual para cada nível (ex.: Nv. 1: 110 pts, Nv.2: 120 pts, Nv. 3: 130 pts, etc)
- Para aumentar o seu nível um explorador deve ganhar pontos de experiência através da ação de explorar.
- Os pontos de experiência devem se manter acumulados mesmo após subir de nível.

## Sobre o ranqueamento:
Um explorador deve ser ranqueado entre 6 ranques diferentes: "Novato", "Explorador", "Veterano", "Elite", "Mestre", "Lenda" (ou qualquer nomenclatura que preferir)
O ranqueamento deve obedecer à seguinte ordem:
- 1-9: Novato
- 10-29: Explorador
- 30-49: Veterano
- 50-79: Elite
- 80-98: Mestre
- 99: Lenda

## Sobre a ação de explorar:
- A ação de explorar precisa de um planeta a ser explorado.
- O planeta a ser explorado precisa ter um id, um nome, um nível de hostilidade (entre pacífico, neutro e hostil) e um tipo de terreno (ex.: desértico, florestal, montanhoso, subaquático, etc).
- Um explorador morto não pode explorar.
- Deve ser possível saber todos os planetas que um explorador já explorou com sucesso.

## Sobre o resultado:
- A ação de explorar pode ser bem sucedida ou falhar. Para determinar o resultado vai ser preciso simular um "rolar de dados", sorteando dois números aleatórios entre 1 e 6, com resultados entre 2 e 12.
- Resultados entre 5 e 12 garantem sucesso em planetas pacíficos.
- Resultados entre 7 e 12 garantem sucesso em planetas neutros.
- Resultados entre 9 e 12 garantem sucesso em planetas hostis.
- Resultado 2 (dois números 1) em planetas hostis o explorador morre (mas não deve ser excluído).
- Após 3 resultados 12 (dois números 6) em planetas de um mesmo terreno o explorador se torna um especialista naquele terreno e recebe um bônus de +1 no resultado dos dados.
- Esse bônus impede que ele morra em caso de falha crítica e aumenta as chances de sucesso.
- Só é possível acumular esse bônus uma vez.

## Sobre os pontos de experiência
Em caso de sucesso na ação de explorar o Explorer deve receber pontos de experiência de acordo com o seguinte:
- 15 pts - Planeta pacífico
- 25 pts - Planeta neutro
- 50 pts - Planeta hostil

Em caso de falha na ação de explorar o Explorer deve receber pontos de experiência de acordo com o seguinte:
- 0 pts - Planeta pacífico
- 0 pts - Planeta neutro
- 10 pts - Planeta hostil

# Testes
Assuma que temos um objeto explorador está no nível 9 e possui 1340 pontos de experiência.
Assuma também que ele já obteve 2 acertos críticos (6+6) explorando terrenos do tipo "forest".
Seu ranque deve ser "Novato"
Assuma que ele explorou um novo planeta { id: 1, name: "Planeta 1", hostility: "neutral", terrain: "forest" }
Ao obter sucesso nessa exploração ele deve:
- Ganhar 25 pontos de exp.
- Avançar para o nível 10.
- Avance para o ranque Explorador.
- Se torne especialista em terrenos "forest" e ganhe o bônus de +1
- Ter o planeta de "Planeta 1" na sua lista de planetas conhecidos.

Assuma agora que ele explorou o planeta { id: 2, name: "Planeta 2", hostility: "hostile", terrain: "desert" } e tirou dois 1 no resultado
Ao obter uma falha crítica nessa exploração ele deve:
- Morrer, se tornando incapaz de explorar novamente.
- O objeto desse explorador ainda deve conter as suas informações.