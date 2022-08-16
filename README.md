# 	:woman_technologist: Project Stranger Things Frontend



Esse projeto contém uma série de informações sobre o que eu aprendi aqui na Trybe ao longo do curso de desenvolvimento web da Trybe. <br>Nele pude desenvolver habilidades como realizar deploy de um projeto front-end usando heroku.

## :rocket:Começando
Esse projeto foi proposto pelo curso de desenvolvimento web da Trybe.
### Desenvolvimento
Foi feito deploy de um projeto front-end com o Heroku, utilizando Docker em ambiente de produção.Para isso, tive que alterar alguns comportamentos aplicando conceitos vistos no conteúdo do bloco.
### Commits
Os commits foram feitos de acordo com os requisitos finalizados.
### Branch
Todo o projeto foi feita na branch 'master', isso por conta da exigência do curso.
### Instalação
Antes de realizar o projeto, precisei instalar as dependências usando npm install.
### Visualização do projeto
O projeto poderá ser visualizado através do comando: $npm start, que vai abrir o http://localhost:3000/ no seu navegador.
### Testes
Os testes usando foram ESLint e Cypress, através dos **comandos**: <br>
* npm run cypress:open <br>
* npm run lint:styles
### Autores
Esse foi um projeto individual,que desenvolvido por Juliana Oliveira.
### Ferramentas usadas
Foi usado Visual Studio Code, além do Trello que auxiliou na organização das tarefas.
### Framework usado
Nenhum.

## :footprints:Requisitos
### Metodologia usada
No trabalho do desenvolvimento de software a gente sempre tem prazos, muitas vezes os prazos são apertados.<br>
Por outro lado, eu não quero criar algo que não entendo perfeitamente, como também fazer códigos rápidos pode levar a erros que podem demorar muito pra corrigir.<br>
Por isso, usei e sempre uso o método Baby Steps, que é uma estratégia de abordar o desafio passo à passo, defensivamente.<br>
Baby steps é um termo em inglês que quer dizer passos de bebê. Refere-se a fazer as coisas, quaisquer que sejam, devagar, com calma, passo a passo.
#### :footprints:Requisito 6 - Verifica as variáveis de ambiente do front-end
Altere o front-end para utilizar variáveis de ambiente para controlar as URLs e Timeouts de comunicação com a API.

Perceba que o código está esperando por duas APIs. Uma para o modo upside-down e a outra para o modo normal.
* Para seu back-end hawkins:<br>REACT_APP_HAWKINS_URL para a URL;<br>REACT_APP_HAWKINS_TIMEOUT para o timeout.<br>
* Para seu back-end UPSIDEDOWN:<br> REACT_APP_UPSIDEDOWN_URL para a URL; <br> REACT_APP_UPSIDEDOWN_TIMEOUT para o timeout.<br>

#### :footprints:Requisito 7 - Verifica se foi feito o deploy do frontend no Heroku
IMPORTANTE: Assim como no Back-end, a variável de ambiente GITHUB_USER deverá ser criada com o seu nome de pessoa usuária do GitHub.
* Crie um app do Heroku com o front-end. Vamos deixar o Heroku utilizar as configurações padrão. No momento de criar o app do Heroku, utilize o buildpack descrito abaixo, em Dicas;
* O nome do seu app no Heroku deve ser seu nome de pessoa usuária do GitHub seguido de "-ft". Por exemplo, se o seu nome de pessoa usuária do GitHub for "student", o nome do seu app será "student-ft" e a URL precisar ser https://student-ft.herokuapp.com/;
* Configure as variáveis de ambiente do app para apontar para as API's publicadas;
* Faça o deploy com o git.
* Para publicar seu front-end React, utilize o buildpack mars/create-react-app.
#### Comandos feitos no requisito 7
heroku buildpacks:set mars/create-react-app<br>
git remote -v // verificar o remote adicionado<br>
heroku stack // verificar o stack disponível<br>
heroku stack:set heroku-20 //mudar pro heroku-20<br>
git add .<br>
git commit -m 'deploy front-end'<br>
git push heroku dev-juliana-oliveira-stranger-things-frontend:master<br>


