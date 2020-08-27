## Banco Capgemini em Laravel

O projeto foi desenvolvido com o Framework [Laravel](http://www.laravel.com) na versão 7.24, e 
[Vue JS](http://www.vuejs.com) no frontend, utilizando API Rest para consulta do saldo 
e interações de depósitos e saques.

As tecnologias propostas são bem conhecidas e com amplo material de consulta, bem como comunidades enormes, 
que podem auxiliar em um problema mais pontual.

Para inclusão dos valores, foi utilizado o componente [vue-currency-input](https://www.npmjs.com/package/vue-currency-input) 
para garantir que o valor inputado pelo usuário seja validado e inserido corretamente.

##INSTALAÇÃO


Clonar repositório

```
$ git clone git@github.com:juniorari/banco-capgemini.git
```

Entrar no diretório

```
$ cd banco-capgemini
```   

Instalar dependências

```
$ composer install
```

Copiar arquivo .env

```
$ cp .env.example .env
```
OBS: O banco está em SQLite no local: `database\database.sqlite`, e caso ainda não tenha
a extensão de conexão com o SQLite, instale com o seguinte comando, trocando o `X` pela 
sua versão do PHP:
```
$ sudo apt install php7.X-sqlite3
```

Gerar a chave da aplicação

```
$ php artisan key:generate
```

Migrations
```
$ php artisan migrate
```

Instalar dependências do node
```
$ npm install
```
```
$ npm run prod
```

Executar servidor

````
php artisan serve 
````

<!--

DESAFIO CAPGEMINI
---  

Roteiro do Desafio 

*** FASE 1 - API Rest *** 

Desenvolvimento da API com os serviços propostos abaixo.  

*** FASE 2 - Frontend em Vue JS *** 

Criar uma tela que seja possível realizar as operações (saldo, depósito e saque).  

O frontend deve consumir a API criada na FASE 1.   

Informações sobre implementação (opcional) 

- Favor informar os seguintes pontos sobre sua implementação: 
1) Faça uma breve descrição sobre a arquitetura utilizada no problema proposto; 
- O projeto foi desenvolvido com o Framework na versão 7.24, e no frontend, utilizando API Rest para consulta do saldo e interações de depósitos e saques.
2) Em sua análise, houve algum problema relevante que gostaria de destacar? 
- Nenhum problema. As tecnologias propostas são bem conhecidas e com amplo material de consulta, bem como comunidades enormes, que nos podem auxiliar em um problema mais pontual. 
3) Houve alguma solução ou padrão arquitetural que tenha aplicado e gostaria de ressaltar?
- Para inclusão dos valores, foi utilizado o componente vue-currency-input para garantir que o valor inputado pelo usuário seja validado e inserido corretamente. 



OBJETIVO DO DESAFIO
---- 

- O Banco Capgemini necessita criar uma Web API Rest para expor os seguintes serviços para 
seus clientes: 
1) Serviço para verificar o saldo de uma conta corrente; 
2) Serviço para realizar um depósito em uma determinada conta corrente; 
3) Serviço para realizar um saque de uma determinada conta corrente.  

REQUISITOS
----

1) A API Rest deve ser desenvolvida no framework Laravel (versão 5.2 ou superior); 
2) O frontend deve ser desenvolvido utilizando Vue JS; 
3) É necessário persistir algum dado, o candidato fica livre para propor a utilização de algum banco de dados. 
Por ter uma melhor portabilidade, sugerimos a utilização do banco em memória SqlLite em memória;  
4) Deve ser utilizado Migrations; 
5) A entrega deverá ser realizada via GitHub. O candidato deverá criar um repositório no GitHub 
para realizar a entrega do projeto (enviar o link ao final do desenvolvimento).  

ANÁLISE
----
 
Serão avaliados os seguintes requisitos:  
1) Solução do problema proposto; 
2) Arquitetura da aplicação e sua distribuição em pacotes; 
3) Legibilidade do código; 
4) Utilização de orientação a objetos; 
5) Melhores práticas de desenvolvimento;
-->
