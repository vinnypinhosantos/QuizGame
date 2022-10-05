# QuizGame
## O que é o jogo?
Esse é um jogo simples de quiz feito no curso 100 Days Of Code.
Consiste em 10 perguntas sobre cinema que o usuário deve responder True ou False.

Todas as perguntas estão em inglês pois foi usada a OpenTriviaData e feita adaptações para um dicionário Python.

## A construção do jogo

### Arquivos
O projeto consiste de quatro arquivos python que usam programação orientada a objetos para criação do código.

#### quiz_brain
Uma classe de controle do funcionamento do programa, que possui os seguintes métodos:
*Construtor: começa o programa pela pergunta n° 0 (question_number = 0), com a pontuação também igual a zero 
e na criação do objeto deve-se ter apenas o parâmetro com a lista de perguntas.
*still_has_questions: verifica se o usuário já respondeu todas as perguntas.
*next_question: formata o texto com o número da questão e a pergunta em si e chama a função check_answer.
*check_answer: verifica se o usuário acertou a resposta ou não. Tem como parâmetros a resposta do usuário
e a resposta correta. Além disso, mostra e controla a pontuação do usuário

#### data
Arquivo que contém os dados das perguntas levantados da [OpenTriviaDataBase](https://opentdb.com/) e adaptados para se 
tornarem um dicionário.

#### question_model
Possui a classe Question que contém o modelo de uma questão. Tem apenas os atributos do número e da resposta.

#### main
Ciclo principal do programa que consiste na criação de uma lista com as perguntas a partir da criação de objetos do tipo
Question e na consequente apresentação e input do usuário enquanto ainda tiver questões para responder.

### Observações e Possíveis melhorias

* O projeto ainda é simples e serve mais para colocar em prática os conceitos aprendidos.
* Os métodos check_answer e next_question podem ser melhorados pois possuem mais de uma função dentro do código.

