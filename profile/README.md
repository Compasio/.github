# Compasio
_Compaixão para o mundo_

A Compasio é uma plataforma sem fins lucrativos para pessoas que buscam se voluntariar em ONG´s e trabalhos voluntários, podendo especificar sua área de atuação. Também possibilitamos que as ONG´s encontrem voluntários ideais para colaborar com seus projetos através das características dos perfis dos usuários.

Somos um projeto desenvolvido com o objetivo de colocar em prática nossos conhecimentos adquiridos durante o Ensino Médio Técnico em Desenvolvimento de Sistemas do SESI/SENAI e apresentá-lo no final do curso.

<br>

## Tech

O projeto utiliza vários tecnologias para funcionar corretamente:

| Nome       | Função                                                                                                            | 
| ---------- | ----------------------------------------------------------------------------------------------------------------- |
| ![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB) | Sistema web responsivo para diferentes plataformas. |
| ![NestJS](https://img.shields.io/badge/nestjs-%23E0234E.svg?style=for-the-badge&logo=nestjs&logoColor=white) | API e sistema de Back-End do projeto.  | 
| ![Prisma](https://img.shields.io/badge/Prisma-3982CE?style=for-the-badge&logo=Prisma&logoColor=white) | ORM para PostgreSQL. | 
| ![Swagger](https://img.shields.io/badge/-Swagger-%23Clojure?style=for-the-badge&logo=swagger&logoColor=white) | Design, Desenvolvimento, Documentação, Teste e Virtualização da API. | 
| ![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=JSON%20web%20tokens) | Sistema de autenticação/autorização de usuário. | 
| ![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white) | Banco de Dados relacional do projeto. |

Nosso projeto é open source com um [repositório público](https://github.com/Compasio) no GitHub.

<br>

## Instalação

Compasio precisa do [Node.js](https://nodejs.org/) em sua versão v21+ para rodar.

Instale todas as dependências necessárias e inicie o servidor:

```sh 
# Na pasta do projeto

# Para instalar as dependências da API e rodá-la
cd backend
npm i
npx prisa migrate dev --name init
npm run start:dev
```
### *Atenção*
Para rodar a API localmente, certifique-se de alterar o arquivo `.env` do projeto para as especificações do seu banco de dados. No exemplo abaixo, é utilizado o usuário `postgres` com a senha `postgres` na porta local 5432. Além disso, tem-se o nome do banco como `minhaDB`.
```sh 
DATABASE_URL="postgresql://postgres:senai@localhost:5432/minhaDB?schema=public"
```

<br>

Como modelo para substituir as informações pelas suas, segue abaixo um link com os espaços onde se deve substituir. 
```sh 
DATABASE_URL="postgresql://<seuUsuario>:<suaSenha>@localhost:<porta>/<nomeDoBanco>?schema=public"
```

<br>

```sh 
# Na pasta do projeto

# Para instalar as dependências do Front-End e rodá-lo
cd frontend
npm i
npm start
```

<br>

_Mais informações sobre a instalação nos repositórios específicos de cada área do projeto (Front-End e Back-End)_
