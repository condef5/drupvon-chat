# React + ES6 + Kemal  Chat Example 

Chat básico construido sobre crystal, react y es6.

## Requirements

* Crystal 0.22.0 
* Node (I have the v7.10.0)
* YARN (I have the v0.24.5)

## Installation

Clona este repositorio :
```sh 
$ git clone https://github.com/condef5/drupvon-chat.git 
$ cd drupvon-chat
```

Antes de correr el programa tienes que instalar las dependencias:

```sh
$ shards install
$ git clone https://github.com/condef5/drupvon-chat.git
$ yarn install
```

## Run Project 

Tú pueddes correr este programa de dos formas:

Compilando/ejecutando el proyecto usando: ` $ crystal build src/app.cr --release`

Corriendo el ejecutable: ` $ ./app `

Una vez que tú corres el programa, tú puedes abrir tu navegador y en [localhost:3000](http://localhost:3000) y ver la actual app.
 
## Deploy

Para subir a producción esta app con heroku, necesitas una cuenta e instalar el toolbet de heroku, antes asegurate de cambiar el socket `ws` por `wss` en client/dist/app.js y ejecutar `$ yarn build` y por último compilar de nuevo el app con `$ crystal build src/app.cr --release`, ahora puedes ejecutar los siguientes comandos pa:

```sh
$ heroku create drupvon-chat --buildpack https://github.com/crystal-lang/heroku-buildpack-crystal
$ git remote -v
$ git add .
$ git commit -m "description of you commit"
$ git push heroku master
```
 