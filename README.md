<h2>Ao baixar use os seguintes comandos</h2>
<code>bundle install</code>
<code>rake db:migrate</code>
 


<h3>Insira sua senha em .env para que tenha acesso ao banco de dados mysql</h3>

<h1>CRUD Simples usando Ruby on Rails</h1>

<h2>Primeiramente criamos o projeto usando mysql<h2>

<code>rails new crud_simples -d mysql</code>


<h2>Criamos o banco de dados

<code>rake db:create</code>
<p>Isso irá gerar 2 banco de dados, um chamado crud_simples_development e o outro é crud_simples_test</p>

<h2>Depois geramos o scaffold School usando g(generate) com as propriedades: name, email e phone com os valores: string, string e integer </h2>
<code>rails g scaffold School name:string email:string phone:integer</code><br>

<h2>Depois migraremos o scaffold pronto para o banco de dados</h2>

<code>rake db:migrate</code>
  <h6>PS:Tive que adicionar o arquivo .env para configurar as variáveis de ambiente, com o nome de my_password como o caso da senha mysql e antes disso adicionei a gem 'dotenv-rails' no gemfile juntamente com o bundle install</h6>
  
 <h2>Depois desse processo é só acessard o seguinte link local </h2>
 <code>localhost:3000/schools</code>
 
 
