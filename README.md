# Node.js - Desafio 3

[![GitHub](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/osvaldokalvaitir/nodejs-desafio3/blob/master/LICENSE)
![](https://img.shields.io/github/package-json/v/osvaldokalvaitir/nodejs-desafio3.svg)
![](https://img.shields.io/github/last-commit/osvaldokalvaitir/nodejs-desafio3.svg?color=red)
![](https://img.shields.io/github/languages/top/osvaldokalvaitir/nodejs-desafio3.svg?color=yellow)
![](https://img.shields.io/github/languages/count/osvaldokalvaitir/nodejs-desafio3.svg?color=lightgrey)
![](https://img.shields.io/github/languages/code-size/osvaldokalvaitir/nodejs-desafio3.svg)
![](https://img.shields.io/github/repo-size/osvaldokalvaitir/nodejs-desafio3.svg?color=blueviolet)
[![made-for-VSCode](https://img.shields.io/badge/Made%20for-VSCode-1f425f.svg)](https://code.visualstudio.com/)
![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)

Aplicação Marketplace usando Node.js, Express, Mongoose, Json Web Token, Nodemailer, Joi, Kue e Sentry.

## Desafio

Nesse terceiro desafio você irá melhorar a aplicação desenvolvida durante o terceiro módulo com as seguintes funcionalidades:

- Armazene as intenções de compra (Purchase) no MongoDB criando um Model e salvando os dados da purchase no método `store` do PurchaseController;
- Crie uma nova rota para o vendedor aceitar uma intenção de compra declarando o item como vendido e a partir desse momento o anúncio não deve ser mais exibido nas listagens e não deve ser mais possível realizar uma intenção de compra para esse anúncio;
- O Ad deve possui um campo adicional chamado `purchasedBy` que armazena o ID da Purchase que o vendedor aceitou, caso esse campo esteja presente, quer dizer que o anúncio foi vendido;

## Índice

- [Desenvolvimento](#desenvolvimento)

  - [Configuração do Ambiente](#configuração-do-ambiente)

  - [Instalação do Projeto](#instalação-do-projeto)

  - [Configuração das Variáveis de Ambiente](#configuração-das-variáveis-de-ambiente)

  - [Execução do Projeto](#execução-do-projeto)

- [Utilizados no Projeto](#utilizados-no-projeto)

  - [Bibliotecas](#bibliotecas)

  - [APIs](#apis)

  - [Ferramentas](#ferramentas)

## Desenvolvimento

### Configuração do Ambiente

Clique [aqui](https://github.com/osvaldokalvaitir/projects-settings/blob/master/README.md) e siga `Configuração de Ambiente`.

### Instalação do Projeto

Clique [aqui](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/nodejs.md) e siga `Instalação de Projeto`.

### Configuração das Variáveis de Ambiente

Clique [aqui](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/dotenv.md) e siga `Configuração de Variáveis de Ambiente`.

### Execução do Projeto

Clique [aqui](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/nodejs.md) e siga `Execução de Projeto para Desenvolvimento` ou `Execução de Projeto para Produção`.

## Utilizados no Projeto

### Bibliotecas

- [@sentry/node](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/@sentry-node.md)

- [bcrypt.js](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/bcryptjs.md)

- [dotenv](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/dotenv.md)

- [ESLint](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/eslint.md)

- [Express](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/express.md)

- [Express Async Handler](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/express-async-handler.md)

- [Express Handlebars](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/express-handlebars.md)

- [Express Handlebars plugin for Nodemailer](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/nodemailer-express-handlebars.md)

- [Express Validation](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/express-validation.md)

- [Joi](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/joi.md)

- [Json Web Token](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/jsonwebtoken.md)

- [Kue](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/kue.md)

- [Mongoose](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/mongoose.md)

- [Mongoose Paginate](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/mongoose-paginate.md)

- [Nodemailer](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/nodemailer.md)

- [Nodemon](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/nodemon.md)

- [requireDir](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/requiredir.md)

- [Youch](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/youch.md)

### APIs

- **Interna**

  - **Rotas**

    - Intenções de Compras

      - Adiciona nova intenção de compra
      - Aceita intenção de compra declarando o item como vendido

    - Anúncios

        - Lista todos os anúncios
        - Lista somente dados de um anúncio
        - Adiciona novos anúncios
        - Edita dados de anúncios existentes
        - Exclui anúncios existentes

    - Sessões

        - Adiciona novas sessões

    - Usuários

        - Adiciona novos usuários

### Ferramentas

- [Docker](https://github.com/osvaldokalvaitir/projects-settings/blob/master/virtualization/docker/docker.md)

  - Imagem do MongoDB: [mongo](https://github.com/osvaldokalvaitir/projects-settings/blob/master/virtualization/docker/images/mongo.md)

  - Imagem do Redis: [redis:alpine](https://github.com/osvaldokalvaitir/projects-settings/blob/master/virtualization/docker/images/redis-alpine.md)

- [Mailtrap](https://github.com/osvaldokalvaitir/projects-settings/blob/master/email/mailtrap.md)

- [Insomnia](https://github.com/osvaldokalvaitir/projects-settings/blob/master/api/insomnia.md)

- [Sentry](https://github.com/osvaldokalvaitir/projects-settings/blob/master/error/sentry.md)
