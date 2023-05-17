## A1_22/2 Prova On-line - Modelagem de Software e Diagramas

# Questão 1
Eu, como usuário, devo poder pegar livros e revistas científicas emprestados e realizar consulta local.
Eu, como funcionário, devo poder os cadastrar os livros e as revistas cientificas no sistema.
Eu, como funcionário, devo poder cadastrar o empréstimo de livros e revistas cientificas.
Eu, como funcionário, posso consultar o status dos empréstimos e devoluções.
Eu, como funcionário, posso registrar o período de empréstimo e a quantidade.
# Questão 2
O site da biblioteca deve ser acessado pelos navegadores MS Edge, Mozila Firefox e Google Chrome.
O sistema deve estar disponível e permitir o uso intenso por até 10 atendentes principalmente nos horários de entrada, intervalos e saída dos alunos. 
O sistema deve estar integrado com o sistema de gestão da Universidade para acessar os dados completos de cadastro dos alunos e professores.
O sistema deve bloquear empréstimos de quantidades de livros superior à permitida dependendo do tipo de usuário (professor ou aluno).
# Questão 3
a. O aluno faz a busca e a reserva de um livro.

Escopo: Livro
Ator Primário: Aluno faz Busca e Reserva de um livro
Stakeholders e Interesses
Aluno: Busca e Reserva de um livro
Livro: Registrar empréstimo
Biblioteca: Emprestar o livro
Empréstimo mínimo: 1 livro
Tempo: Quantidade máxima de dias do empréstimo
Pré-Condição: Estar Cadastro como aluno na faculdade
Cenário de sucesso principal: 
- Aluno faz a busca do livro
- Aluno seleciona para fazer a reserva os livros desejados
- Aluno escolhe a quantidade de dias dentro do limite de dias para empréstimo
- Aluno clica para finalizar o empréstimo
- Aluno retira o livro com o bibliotecário ou atendente
- Aluno deve receber um e-mail com os dados do empréstimo
Extensões:
1. Aluno faz a busca de um livro não disponível.
    1a. Sistema informa que o livro estará disponível em provável data de devolução.
    2a.  Sistema informa que não tem nenhuma unidade do livro no acervo da biblioteca.
2. Aluno seleciona para reservar os livros desejados.
     2a. Sistema irá registrar o empréstimo do livro, para que quando disponível esse aluno ser o próximo a pegar o livro. 


b. O funcionário registra o empréstimo de um livro.

Escopo: Livro
Ator Primário: Funcionário registra o empréstimo de um livro
Stakeholders e Interesses
Funcionário: Registra o empréstimo de um livro
Aluno: Solicita Reserva de um livro
Livro: Registrar empréstimo
Biblioteca: Emprestar o livro
Empréstimo mínimo: 1 livro
Tempo: Quantidade máxima de dias do empréstimo.
Pré-Condição: Estar Cadastro como Funcionário na Biblioteca
Cenário de sucesso principal: 
- Funcionário verifica o cadastro do aluno através do nome e número de matricula.
- Funcionário busca o livro.
- Funcionário verifica a disponibilidade.
- Funcionário registra o empréstimo.
- Funcionário entrega o livro ao aluno.
Extensões:
1. Funcionário verifica que não existe o cadastro do aluno através do nome e número de matricula.
    1a. Funcionário irá informar que é necessário que o aluno se cadastra na secretaria da faculdade para constar no sistema.
2. Funcionário busca um livro indisponível.
    2a. Funcionário irá informar que o livro está emprestado e por isso pode apenas reservar e verificar quando será a provável data de devolução.
    2b. Funcionário irá informar ao aluno que a biblioteca não possui o Livro desejado pelo aluno.
Pré-Condições: O usuário deverá estar autenticado no sistema. 
Cenário Principal  
1. O Sistema solicita os dados necessários para realizar o empréstimo. 
2. O Funcionário pesquisa o livro solicitado pelo aluno.
3. O Funcionário pesquisa o cadastro do aluno.
4. O Funionário seleciona a opção de reservar com as informações de usuário e livro selecionadas.
5. O Funcionário clica em reservar. 
6. O Sistema emite uma mensagem “Empréstimo realizado com êxito”. 
7. O Sistema salva o Empréstimo. 
Cenário Alternativo: O Usuário poderá cancelar o processo durante a movimentação.
