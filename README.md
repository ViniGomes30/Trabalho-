# TG0 - Desenvolvimento de Sistemas I

## Proposta de Tema e Apresentação da Equipe

### Autores
* Alan Ribeiro do Carmo, TIA: 42370086, RA: 10428496
* Lucas Alves de Paula, TIA: 42303990, RA: 10408837
* Hittalo Gabriel Asevedo Silva, TIA: 42315476, RA: 10426383
* Vinicius Gutierrez Gomes, TIA: 42306779, RA: 10425609

## Descrição do Projeto
Nosso projeto visa atender à necessidade comum de muitas pessoas que desejam preparar uma refeição deliciosa, mas estão indecisas sobre qual receita seguir ou estão limitadas pelos ingredientes disponíveis em suas geladeiras. Para resolver esse problema, estamos desenvolvendo um aplicativo de receitas inovador que permite aos usuários encontrar receitas com base nos ingredientes que têm em casa.

O aplicativo terá uma interface simples e intuitiva, onde os usuários poderão inserir os ingredientes que possuem em sua despensa ou geladeira. Em seguida, o aplicativo realizará uma pesquisa em nosso banco de dados abrangente de receitas e retornará uma lista de receitas que podem ser preparadas com os ingredientes fornecidos pelo usuário.

1. Necessidade de descobrir uma receita com os ingredientes disponíveis.
2. É comum se ver numa situação em que você quer comer algo específico mas não sabe o que fazer, ou você quer fazer uma receita nova que nunca tinha feito antes, além de que muitas vezes você não tem muitos ingredientes, então vimos a necessidade de fazer esse aplicativo que acha a receita de acordo com os ingredientes que o usuário tiver.
3. Nesse software, o usuário vai digitar os ingredientes que ele tem em casa e vai ser feita uma pesquisa no banco de receitas que vai mostrar as receitas que ele pode fazer com aqueles ingredientes.
4. Qualquer pessoa que deseja fazer uma receita mas não tem certeza do que pode ser feito com o que ele tem disponível.
5. **Requisitos de Qualidade:**
   - Precisão na correspondência de receitas com os ingredientes disponíveis.
   - Interface intuitiva e fácil de usar.
   - Velocidade de resposta do aplicativo.
   - Disponibilidade de uma ampla variedade de receitas.
   - Atualização regular do banco de dados de receitas e ingredientes.
   - Segurança e privacidade dos dados dos usuários.

6. **Riscos:**
   - O programa não fazer a pesquisa corretamente e mostrar receitas incompatíveis.
   - Receitas de baixa qualidade podem ser exibidas, resultando em insatisfação do usuário.

## Canvas
![Canvas](https://github.com/ViniGomes30/Trabalho-/assets/126883066/444db95e-e439-4379-a998-38c3be4cf25d)

## Especificação de Caso de Uso
| Identificador | AHLV                 |
|---------------|----------------------|
| Nome          | Gerador de Receitas  |
| Atores        | Usuário              |
| Sumário       | O usuário irá inserir os ingredientes que ele tem disponível em sua casa e o sistema irá pesquisar entre as receitas disponíveis, qual o usuário poderá fazer com os ingredientes que ele possui. |
| Pré-condição  | O usuário deve informar a quantidade mínima de ingredientes. |
| Pós-condição  | O sistema informa alguma(s) receita(s). |

### Fluxo Principal
| Ações do Ator                                      | Ações do Sistema                                                                                   |
|----------------------------------------------------|----------------------------------------------------------------------------------------------------|
| 1. O usuário clica no botão “Inserir ingredientes” | 2. O sistema apresenta 2 opções para o usuário:                                                                                                                           |
|                                                    |    - “Pesquisar receitas que são necessários APENAS esses ingredientes”                                                                  |
|                                                    |    - “Pesquisar receitas com esses ingredientes, mas que possa ter mais outros”                                                            |
| 3. O usuário escolhe a opção desejada              |                                                                                                    |
|                                                    | 4. O sistema faz a pesquisa de acordo com a opção e os ingredientes desejados                        |
|                                                    | 5. O sistema apresenta as opções de receitas disponíveis.                                            |
|                                                    |    - Caso de uso é encerrado.                                                                     |

### Fluxo Alternativo 1: A opção selecionada é “Pesquisar receitas que são necessários APENAS esses ingredientes”
| Ações do Ator                              | Ações do Sistema                                                                                                                                   |
|--------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------|
|    | 3.1.1. O sistema apresenta diversas opções que o usuário pode escolher, além de apresentar uma barra de pesquisa, e solicita ao usuário que insira pelo menos 2 ingredientes que deseja utilizar. |
| 3.1.2. O usuário clica em "pesquisar receitas" |                                                                                                                                                   |
|                                            | 3.1.3. O sistema volta ao passo 4 do fluxo principal                                                                                               |

### Fluxo Alternativo 2: A opção selecionada é “Pesquisar receitas com esses ingredientes, mas que possa ter mais outros”
| Ações do Ator                              | Ações do Sistema                                                                                                                                   |
|--------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------|
| 3.2.2. O usuário escolhe os ingredientes que ele possui e clica em “pesquisar receitas” | 3.2.1. O sistema apresenta diversas opções que o usuário pode escolher, além de apresentar uma barra de pesquisa, e solicita ao usuário que insira pelo menos 1 ingrediente desejado. |
|                                            | 3.2.4. O sistema volta ao passo 4 do fluxo principal                                                                                               |

## Diagramas de Classe

### Gerador de Receitas
| Método                   |
|--------------------------|
| inserirIngredientes(): void |
| pesquisarReceitas(): void |
| listarReceitas(): void   |           

### Receita
| Atributos                 |
|--------------------------|
| - nome: String           |
| - ingredientes: List<String> |
|--------------------------|
| + getNome(): String      |
| + getIngredientes(): List<String>|

## Diagramas de Sequência
![Imagem do WhatsApp de 2024-04-25 à(s) 12 32 37_cbb5306d](https://github.com/ViniGomes30/Trabalho-/assets/126883066/f51c7c7e-429a-47b7-87cc-64481e34b570)

## Diagramas de Atividade 
![Imagem do WhatsApp de 2024-05-02 à(s) 22 28 31_cb1a0e91](https://github.com/ViniGomes30/Trabalho-/assets/126883066/499d8b81-9ec0-4dde-a47c-9b2278e44fb4)

## Diagramas de Transição de Estados

![image](https://github.com/ViniGomes30/Trabalho-/assets/126883066/4e1e2b65-48b3-48ce-a1ec-44f5d99eb16a)

## Representação 
![Representação](https://github.com/ViniGomes30/Trabalho-/assets/126883066/d912efe2-35f2-4bd1-bd47-6a8ef12e6663)
