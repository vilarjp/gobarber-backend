
# GoBarber - back end

Sistema de CRUD seguindo o modelo API REST para ser consumido futuramente pelo GoBarber - front end.

### Detalhes da aplicação:

- [sentry](https://sentry.io/for/node/) para registro de logs de erro em tempo real
- [bcryptjs](https://github.com/dcodeIO/bcrypt.js/) para encriptação da senha dos usuários
- [bee-queue](https://bee-queue.com/) para gerir job queues na aplicação
- [handlebars](https://handlebarsjs.com/) para gerar os templates de e-mail
- [jsonwebtoken](https://github.com/auth0/node-jsonwebtoken#readme) para gerar e validar o token de autenticação
- [moongose](https://mongoosejs.com/) como ODM para o MongoDB
- [multer](https://github.com/expressjs/multer#readme) para gerir o upload de arquivos para o servidor
- [nodemailer](https://nodemailer.com/about/) para gerir o envio de e-mail
- [sequelize](https://sequelize.org/) como ORM para o PostgreSQL
- [youch](https://github.com/poppinss/youch#readme) para tratar erros como Promises
- [yup](https://github.com/jquense/yup) para criar modelos de schemas para validação dos dados recebidos pela aplicação

- [postgresql](https://www.postgresql.org/) como banco de dados principal da aplicação
- [mongodb](https://www.mongodb.com/) como banco de dados secundário da aplicação, para gerir as notificações
- [redis](https://redis.io/) como banco de dados para auxiliar as job queues de envio de e-mail da aplicação

- [docker](https://www.docker.com/) como container para as imagens dos bancos de dados da aplicação

### Rotas:

- /providers/:id/available GET
- /notifications GET
- /notifications/:id PUT
- /schedule GET
- /sessions POST
- /files POST
- /appointments POST
- /appointments/:id DELETE
- /appointments GET
- /providers GET
- /users POST
- /users PUT

## Principais Comandos

### Instalar dependencias do projeto
```
:~$ cd <pasta do projeto>
:~$ yarn
```
### Como executar o projeto?
```
:~$ yarn dev
```
### Para executar e manter em funcionamento a fila de e-mails
```
:~$ yarn queue
```
