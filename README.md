# Be the hero
Sistema desenvolvido durante a Semana Omni Stack 11, que visa ajudar ONGs com doações.

<p align="center">
  <img src="https://github.com/carlosguttemberg/be-the-hero/blob/master/frontend/src/assets/heroes.png" width="600">
</p>

<hr>

### :scroll: Sobre o projeto

<p>O projeto foi desenvolvido durante a semana Omnistack 11, tem por objetivo ajudar as ONGs a pagarem as contas de determinados procedimentos</p>
<p>Com isso foram construido três aplicações, uma usando NodeJs para servidor, outra usando React como Frontend da web e uma feita com React Native
para aplição mobile além do CSS feito especificamente para o projeto</p>

<p align="center">
   <img src="https://github.com/carlosguttemberg/Pokedex/blob/master/img/node-js.png" width="400">
   <img src="https://github.com/carlosguttemberg/Pokedex/blob/master/img/react.png" width="400">
</p>

<p>O projeto web conta com uma tela de login onde deve ser informado o código da ONG que está se autenticando</p>

<p align="center">
   <img src="https://github.com/carlosguttemberg/be-the-hero/blob/master/img/login.png" width="1200">
</p>

<p>Após autenticado cada ONG poderá visualizar os casos já cadastrados, deletar alguns casos ou cadastrar novos casos</p>

<p align="center">
   <img src="https://github.com/carlosguttemberg/be-the-hero/blob/master/img/listOfCases.png" width="1200">
   <img src="https://github.com/carlosguttemberg/be-the-hero/blob/master/img/newCase.png" width="1200">
</p>

<p>Navegação entre as telas do projeto Web</p>
<p align="center">
  <img src="https://github.com/carlosguttemberg/be-the-hero/blob/master/img/login.gif" width="1200">
  <img src="https://github.com/carlosguttemberg/be-the-hero/blob/master/img/newCase.gif" width="1200">
</p>

<p>O projeto mobile é destinado as pessoas que desejam entrar em contato com a ONG para poder ajudar com o pagamento de determinados casos</p>
<p>Ao acessar o aplicativo o usuário visualizará a splash screen da aplicação, e logo após os casos das ONGs</p>
<p align="center">
  <img src="https://github.com/carlosguttemberg/be-the-hero/blob/master/img/splashScreen.png" width="400" height="800px">
  <img src="https://github.com/carlosguttemberg/be-the-hero/blob/master/img/mobListOfCases.png" width="400" height="800px">
</p>

<p>Ao selecionar um dos casos o usuário poderá enviar um email ou mensagem pelo Whatsapp da ONG</p>
<p align="center">
  <img src="https://github.com/carlosguttemberg/be-the-hero/blob/master/img/contactOng.png" width="400" height="800px">
</p>

<p>Navegação entre as telas do projeto Mobile, a paginação é feita usando o InfiniteScroll, onde ao chegar ao final da pagina mais casos serão carregados</p>
<p align="center">
  <img src="https://github.com/carlosguttemberg/be-the-hero/blob/master/img/mobInfiniteScroll.gif" width="400" height="800px">
  <img src="https://github.com/carlosguttemberg/be-the-hero/blob/master/img/mobNavigation.gif" width="400" height="800px">
</p>

### :rocket: Executando o projeto
<p>Primeiro é preciso instalar as dependencias dos projetos, para isso basta acessar as pastas backend, frontend e mobile pelo terminal e executar o install</p>

```bash
  npm install
```
### :factory: Executando o servidor (Aplicação em NodeJs)
<p>Por padrão a aplicação já esta com uma base de dados SQLite sendo enviada junto ao projeto, porém pode ser criado uma nova em outra base de dados, 
para isso basta acessar o arquivo knexfile.js e alterar as configurações. Mais informações na documentação http://knexjs.org/</p>

<p>Depois de configurado acesse a pasta backend pelo terminal, será preciso executar a criação das tabelas na base de dados, executando o comando:</p>

```bash
  npx knex migrate:latest
```
<p>Feito isso só será preciso executar o comando abaixo na pasta do backend para que o servidor fique rodando, ele funciona na porta 3333</p>

```bash
  npm start
```

### :computer: Executando o Frontend (React)
<p>Na aplicação react só será preciso executar o start, na pasta frontend e o site será carregado</p>

```bash
  npm start
```

### :computer: Executando a aplicação Mobile (React Native)

<p>Primeiro sera preciso acessar pelo terminal a pasta mobile, executar o start</p>

```bash
  npm start
```

<p>No navegador sera gerado um QRCode, que deverá ser lido pela camera do aparelho iOS ou Android, lembrando que precisa que o 
aplicativo expo esteja instalado no aparelho. Feito isso a aplicação sera carregada no aparelho</p>

<p align="center">
  <img src="https://github.com/carlosguttemberg/be-the-hero/blob/master/img/qrCodeExpo.png" width="1200">
</p>
