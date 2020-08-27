Banco Capgemini em Laravel
----

O projeto foi desenvolvido com o Framework [Laravel](http://www.laravel.com) na versão 7.24, e 
[Vue JS](http://www.vuejs.com) no frontend, utilizando API Rest para consulta do saldo 
e interações de depósitos e saques.

As tecnologias propostas são bem conhecidas e com amplo material de consulta, bem como comunidades enormes, 
que podem auxiliar em um problema mais pontual.

Para inclusão dos valores, foi utilizado o componente [vue-currency-input](https://www.npmjs.com/package/vue-currency-input) 
para garantir que o valor inputado pelo usuário seja validado e inserido corretamente.

INSTALAÇÃO
----


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
