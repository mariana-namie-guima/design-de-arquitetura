# Exemplo de Design de Arquitetura

![exemplo_arq.jpg](https://github.com/kterra/Inteli-2024-1B/blob/main/materiais/ponderada-2/exemplo-arq-v2.jpg)

Link de download Draw.io: (https://drive.google.com/file/d/1hQliuMZirU0yiKzAr0d_5koE5qVwEQ2K/view?usp=sharing) 

# Template Readme para Arquitetura MVC em Markdown
- Nome do Projeto: WebCulture
- Descrição: o projeto é um website que busca melhorar a comunicação entre os estudantes que participam do jogo Cesim Global Challenge e demontrar seu desempenho, por meio de feedbacks dos colegas e de uma autoavaliação
- Arquitetura: MVC (Model-View-Controller)
- Ferramenta de Diagramação: draw.io

### Modelos (Models):
- Descreva as entidades do seu projeto e seus atributos.
- Explique as relações entre as entidades.

O "Models" foi dividido em três entidades: login, user, avaliação. No quadro do login, há os atributos "usuário" e "senha", que pegam os valores digitados para serem comparados com os valores no banco de dados. 

### Controladores (Controllers):
- Liste os controladores do seu projeto e suas responsabilidades.
- Descreva as ações (methods) de cada controlador e seus parâmetros de entrada e saída.
- Explique como os controladores interagem com os modelos e views.

### Views (Views):

&nbsp;&nbsp;&nbsp;&nbsp;As Views estão divididas em 5 telas: cadastro, login, perfil, avaliações e feedback.
<br>
&nbsp;&nbsp;&nbsp;&nbsp;Na tela de cadastro, há um header indicando para o usuário em qual tela ele está, seguido por um formulário para inserir seus dados pessoais (nome, idade, nacionalidade, gênero e biografia). Por fim, há um botão para savar as informações e terminar o cadastro. Já na tela de login, há outro header indicando que o usuário está na tela tela de login. Abaixo, há dois "textarea" para inserir o login e a senha e há um botão para realizar o login no fim da página.
<br>
&nbsp;&nbsp;&nbsp;&nbsp;Dentro do site, a tela de perfil é indicada por um header e mostra as informações preenchidas durante os cadastro em um parágrafo. Além disso, há também uma agenda/tabela para preencher quais horários o usuário está livre. Na tela de avaliações, há um formulário para responder as avaliações e um botão para enviá-las. Por fim, existe a tela de feedback que possui com header "Feedback" e um gráfico com as avalições de pares e autoavaliações.

### Infraestrutura:

- Descreva os componentes de infraestrutura do seu projeto, como bancos de dados, APIs externas e outras dependências.
- Explique como a infraestrutura se integra à arquitetura MVC.


### Justifique as escolhas feitas e como elas impactam o projeto.
#### Implicações da Arquitetura:
Descreva as implicações da arquitetura em termos de escalabilidade, manutenção, testabilidade e outros aspectos importantes.

### Recursos Adicionais:
- Documentação do Sails.js: https://github.com/balderdashy/sails
- Tutorial do draw.io: https://m.youtube.com/watch?v=w3zm-wbmlpc
- Exemplos de diagramas MVC: https://www.lucidchart.com/pages/templates

