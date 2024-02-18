Description
-
This is an API REST, to control a polling result. With this application, you'll be able to create a poll with its options, show an
specific poll details and voting on some poll.
You can vote only once in some option. If you choose to vote on another option, your previously vote will be removed and counted on
the other option.

This project uses the following technologies:
- 
- NodeJS as backend application
- Typescript to enforce types and a better structured backend
- Fastify as to make faster http server requests
- Zod library for request validation
- Prisma ORM to interact with databases
- Postgres as database
- Redis as cached database to store and retrieve the voting faster
- Websockets to listen in real time the voting results of a poll
- Docker to mount and run postgres, redis images on your local development environment

Installation
-

To install this project on your machine, you must clone this repository, have both Docker and NodeJS installed on your setup.

```bash
$ npm install
```

Running project
-

```bash
$ docker compose up
```

```bash
$ npm run dev
```

```bash
$ npx prisma migrate dev
```

- Command available by Prisma Client, to view records stored in database, on the browser

```bash
$ npx prisma studio
```
