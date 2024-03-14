# TG0 - Desenvolvimento de Sistemas I
Proposta de Tema e apresentação da Equipe.

# Autores 
* Alan Ribeiro do Carmo, Tia: 42370086, RA: 10428496
* Lucas Alves de Paula, Tia: 42303990, RA: 10408837
* Hittalo Gabriel Asevedo Silva, Tia: 42315476, RA: 10426383
* Vinicius Gutierrez Gomes, Tia: 42306779, RA: 10425609

# Descrição do projeto
Nosso projeto visa atender a necessidade comum de muitas pessoas que desejam preparar uma refeição deliciosa, mas estão indecisas sobre qual receita seguir ou estão limitadas pelos ingredientes disponíveis em suas geladeiras. Para resolver esse problema, estamos desenvolvendo um aplicativo de receitas inovador que permite aos usuários encontrar receitas com base nos ingredientes que têm em casa. 
O aplicativo terá uma interface simples e intuitiva, onde os usuários poderão inserir os ingredientes que possuem em sua despensa ou geladeira. Em seguida, o aplicativo realizará uma pesquisa em nosso banco de dados abrangente de receitas e retornará uma lista de receitas que podem ser preparadas com os ingredientes fornecidos pelo usuário.

1 - Necessidade de descobrir uma receita com os ingredientes disponíveis.

2 - É comum se ver numa situação em que você quer comer alguma coisa específica mas não sabe o que fazer, ou você quer fazer uma receita nova que nunca tinha feito antes, além de que muitas vezes você não tem muitos ingredientes, então vimos a necessidade de fazer esse aplicativo que acha a receita de acordo com os ingredientes que o usuário tiver.

3 - Nesse software, o usuário vai digitar os ingredientes que ele tem em casa e vai ser feita uma pesquisa no banco de receitas que vai mostrar as receitas que ele pode fazer com aqueles ingredientes.

4 - Qualquer pessoa que deseja fazer uma receita mas não tem certeza do que pode ser feito com o que ele tem disponível.

5 - 
* Precisão na correspondência de receitas com os ingredientes disponíveis.
* Interface intuitiva e fácil de usar.
* Velocidade de resposta do aplicativo.
* Disponibilidade de uma ampla variedade de receitas.
* Atualização regular do banco de dados de receitas e ingredientes.
* Segurança e privacidade dos dados dos usuários.

6 - Os riscos não são muito prejudiciais para o usuário, mas pode acontecer: o programa não fazer a pesquisa do jeito certo e mostrar receitas incompatíveis, ou pode ter receitas que não são tão boas, dessa forma o usuário pode ficar insatisfeito com a aplicação e pode acabar desinstalando.

# Canvas 
![image](https://github.com/ViniGomes30/Trabalho-/assets/126883066/444db95e-e439-4379-a998-38c3be4cf25d)

# Especificação de caso de uso
| Identificador | AHLV    |
|---------------|---------|
| Nome          | Procurador de Receita |
| Atores        | Usuário |
| Sumário       | O usuário irá inserir os ingredientes que ele tem disponível em sua casa e o sistema irá pesquisar entre as receitas disponíveis, qual o usuário poderá fazer com os ingredientes que ele possui. |
| Pré-condição  | O usuário deve informar a quantidade mínima de ingredientes. |
| Pós-condição  | O sistema informa alguma(s) receita(s). |
| Pontos de Inclusão | - |
| Pontos de Extensão | - |

# Fluxo Principal
| Ações do Ator                                      | Ações do Sistema                                                                                   |
|----------------------------------------------------|----------------------------------------------------------------------------------------------------|
| 1. O usuário clica no botão “Inserir ingredientes” | 2. O sistema apresenta 2 opções para o usuário:                                                                                                                           |
|                                                    |    - “Pesquisar receitas que são necessários APENAS esses ingredientes”                                                                  |
|                                                    |    - “Pesquisar receitas com esses ingredientes, mas que possa ter mais outros”                                                            |
| 3. O usuário escolhe a opção desejada              |                                                                                                    |
|                                                    | 4. O sistema faz a pesquisa de acordo com a opção e os ingredientes desejados                        |
|                                                    | 5. O sistema apresenta as opções de receitas disponíveis.                                            |
|                                                    |    - Caso de uso é encerrado.                                                                     |


# Fluxo Alternativo 1: A opção selecionada é “Pesquisar receitas que são necessários APENAS esses ingredientes”
| Ações do Ator                                       | Ações do Sistema                                                                                                                                                            |
|-----------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1. O usuário clica no botão “Inserir ingredientes” | 2. O sistema apresenta 2 opções para o usuário:                                                                                                                                                                                         |
|                                                     |    - “Pesquisar receitas que são necessários APENAS esses ingredientes”                                                                                                                                                                  |
|                                                     |    - “Pesquisar receitas com esses ingredientes, mas que possa ter mais outros”                                                                                                                                                            |
| 3. O usuário escolhe a opção desejada               |                                                                                                                                                                             |
|                                                     | 3.1.1. O sistema apresenta diversas opções que o usuário pode escolher, além de apresentar uma barra de pesquisa, após isso, o sistema solicita que o usuário insira ao menos 2 ingredientes que o usuário deseja utilizar. |
| 3.1.2. O usuário escolhe os ingredientes           |                                                                                                                                                                             |
|                                                     | 3.1.3. O sistema volta ao passo 4 do fluxo principal                                                                                                                                                                                     |
| 4.                                                   | O sistema faz a pesquisa de acordo com a opção e os ingredientes desejados                                                                                                                                                              |
| 5.                                                   | O sistema apresenta as opções de receitas disponíveis.                                                                                                                                                                                   |
|                                                     |    - Caso de uso é encerrado. |

# Fluxo Alternativo 2: A opção selecionada é “Pesquisar receitas com esses ingredientes, mas que possa ter mais outros”
| Ações do Ator                                       | Ações do Sistema                                                                                                                                                           |
|-----------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1. O usuário clica no botão “Inserir ingredientes” | 2. O sistema apresenta 2 opções para o usuário:                                                                                                                                                                                        |
|                                                     |    - “Pesquisar receitas que são necessários APENAS esses ingredientes”                                                                                                                                                                 |
|                                                     |    - “Pesquisar receitas com esses ingredientes, mas que possa ter mais outros”                                                                                                                                                           |
| 3. O usuário escolhe a opção desejada               |                                                                                                                                                                            |
|                                                     | 3.1.1. O sistema apresenta diversas opções que o usuário pode escolher, além de apresentar uma barra de pesquisa, após isso, o sistema solicita que o usuário insira ao menos 2 ingredientes que o usuário deseja utilizar. |
| 3.1.2. O usuário escolhe os ingredientes           |                                                                                                                                                                            |
|                                                     | 3.1.3. O sistema volta ao passo 4 do fluxo principal                                                                                                                                                                                    |
| 3.2.2. O usuário escolhe os ingredientes           |                                                                                                                                                                            |
|                                                     | 3.2.4. O sistema volta ao passo 4 do fluxo principal                                                                                                                                                                                    |
| 4.                                                   | O sistema faz a pesquisa de acordo com a opção e os ingredientes desejados                                                                                                                                                             |
| 5.                                                   | O sistema apresenta as opções de receitas disponíveis.                                                                                                                                                                                  |
|                                                     |    - Caso de uso é encerrado.                                                                                                                                                                                                         |






