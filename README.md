# Exemplo de Design de Arquitetura

![exemplo_arq.jpg](https://github.com/mariana-namie-guima/design-de-arquitetura/blob/main/design_de_arquitetura.drawio)

Link de download Draw.io: (https://drive.google.com/file/d/1hQliuMZirU0yiKzAr0d_5koE5qVwEQ2K/view?usp=sharing) 

# Template Readme para Arquitetura MVC em Markdown
- Nome do Projeto: WebCulture
- Descrição: o projeto é um website que busca melhorar a comunicação entre os estudantes que participam do jogo Cesim Global Challenge e demontrar seu desempenho, por meio de feedbacks dos colegas e de uma autoavaliação
- Arquitetura: MVC (Model-View-Controller)
- Ferramenta de Diagramação: draw.io

### Modelos (Models):

&nbsp;&nbsp;&nbsp;&nbsp;O "Models" foi dividido em três entidades: login, user, avaliação. No quadro do login, há os atributos "usuário" e "senha", que pegam os valores digitados para serem comparados com os valores no banco de dados. Já na entidade "Users", os valores colocados no formulários de cadastro são atribuídos aos atributos nome, idade, nacionalidade, gênero e biografia; o quais ão armazenados no banco de dados. Posteriormente, esses valores podem ser chamados pela tela "Perfil" a fim de mostrar alguns dados básicos do usuário. Por fim, na área "Avaliação" os resultados dos formulários de avaliações são armazenados e enviados para o banco de dados, o qual pode ser acessado para mostrar od feedbacks.

### Controladores (Controllers):

&nbsp;&nbsp;&nbsp;&nbsp; O projeto tem 2 controladores: o User e a Avaliação. No primeiro controlador, há o método "Cadastrar" que recebe as informações inputadas na tela de cadastro e as armazena no model "User". O método "Fazer login" recebe os dados inputados na tela de login e os envia para o model "Login", que compara com as informações de login e senha no banco de dados. O método "Mostrar perfil" é ativado quando a botão para a tela de perfil é pressionada e mostra como output as informações do model "User". Por fim, o método "Atualizar" recebe os horários escolhido na agenda pelo usuário e atualiza o tributo "Agenda" com o novo horário.

&nbsp;&nbsp;&nbsp;&nbsp; No controlador "Avaliação", há o método enviar, o qual envia os inputs do forms de avaliação para o model "Avaliação", para que as respostas sejam armazenadas em um banco de dados. Também há o método "Receber feedback", que pega as informações da avaliação de pares e da autoavaliação do banco de dados e as envia para a tela de feedback a fim de serem visualizadas. 

### Views (Views):

&nbsp;&nbsp;&nbsp;&nbsp;As Views estão divididas em 5 telas: cadastro, login, perfil, avaliações e feedback. Na tela de cadastro, há um header indicando para o usuário em qual tela ele está, seguido por um formulário para inserir seus dados pessoais (nome, idade, nacionalidade, gênero e biografia). Por fim, há um botão para savar as informações e terminar o cadastro. Já na tela de login, há outro header indicando que o usuário está na tela tela de login. Abaixo, há dois "textarea" para inserir o login e a senha e há um botão para realizar o login no fim da página.

&nbsp;&nbsp;&nbsp;&nbsp;Dentro do site, a tela de perfil é indicada por um header e mostra as informações preenchidas durante os cadastro em um parágrafo. Além disso, há também uma agenda/tabela para preencher quais horários o usuário está livre. Na tela de avaliações, há um formulário para responder as avaliações e um botão para enviá-las. Por fim, existe a tela de feedback que possui com header "Feedback" e um gráfico com as avalições de pares e autoavaliações.

### Infraestrutura:

&nbsp;&nbsp;&nbsp;&nbsp; No projeto, os dados serão armazenados no banco de dados Postgre e serão visualizados e manipulados por meio do Dbeaver. Além disso, utilizaremos o Render para brigar o servidor do nosso website. Em relação ao frontend, serão utilizadas as linguagens CSS, HTML e JavaScript. Já no backend, será utilizado o Sails, para organizar as pastas do projeto no modelo MVC, e o Node.js, que possibilita a utilização do JavaScript no backend.

### Justifique as escolhas feitas e como elas impactam o projeto.
#### Implicações da Arquitetura:

&nbsp;&nbsp;&nbsp;&nbsp;Para testar a nossa arquitetura, deveremos criar um perfil com um usuário e senha para testar o cadastro e o login. Em seguida, devemos testar se as informações colocadas no formulário de cadastro aparecem na tela de perfil. Nessa mesma tela, deve-se ver se os horário marcados na agenda são salvos após fechá-la. Por fim, devemos testar se as respostas das avaliações são salvas e visualizadas na tela de feedback.
&nbsp;&nbsp;&nbsp;&nbsp;Como utilizaremos o modelo MVC, esperamos que a manutenção do website seja simples, uma vez que haverá uma boa organização dos arquivos que o compõem, sendo o mesmo válido para a escalabilidade.

### Recursos Adicionais:
- Documentação do Sails.js: https://github.com/balderdashy/sails
- Tutorial do draw.io: https://m.youtube.com/watch?v=w3zm-wbmlpc
- Exemplos de diagramas MVC: https://www.lucidchart.com/pages/templates

