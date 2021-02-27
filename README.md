# NLW#4-Rocketseat

## Sistema de envio de pesquisa via email e obtenção do cálculo do NPS

### Utilizado:

<p align="left" >
	
#### Bibliotecas:
- Yup
- uuid
- Nodemailer
- Handlebars
- Reflect-metadata
- Express-async-errors
- Supertest

</p>

<p align="right" >

#### Frameworks:
- NodeJS
- Express
- Jest

</p>
<p align="right" >

#### Linguagens:
- Typescript
- SQL

#### ORM:
- TypeORM
 
#### Banco de Dados:
- Sqlite

</p>
 <p align="right" >
 
#### Aplicações:
- Insomnia
- Ethereal Email
- Beekeeper
- VSCode
</p>
<hr />

## Aprendizados

Gostaria de destacar os aprendizados que tive nesse projetos:
- Como customizar de Erros e validações
- Como definir configurações em json
- Como construir uma aplicação para o envio de email
- Como construir um template de email
- Conheci algumas ferramentas e bibliotecas novas
- Conceitos de rotas, repositorio, views e models mais consolidados

<hr />

## Definições de POST e GET para utilizar a API:

### POST
/users

```
{
	"nome": "Strongreen",
	"email": "strongreen@live.com"
}
```

### GET
/users

```
[
  {
    "id": "33fce935-8ff5-4e73-8b1e-71ad3355b9a9",
    "name": "Strongreen",
    "email": "strongreen@live.com",
    "created_at": "2021-02-27T16:31:14.000Z"
  },
  {
    "id": "e7580421-d646-4605-a8fa-1b87a55bd23f",
    "name": "Strongreen2",
    "email": "strongreen2@live.com",
    "created_at": "2021-02-27T18:59:23.000Z"
  }
]
```

### POST
/surveys

```
{
	"title": "Queremos ouvir a sua opnião",
	"description": "De 0 a 10 quanto você recomendaria a Rocketseat?"
}
```

### GET
/surveys

```
[
  {
    "id": "f101a328-8fd4-431b-9b3d-78ecf56a2f1a",
    "title": "Queremos ouvir a sua opnião",
    "description": "De 0 a 10 quanto você recomendaria a Rocketseat?",
    "created_at": "2021-02-27T16:31:08.000Z"
  },
  {
    "id": "750c9f71-f765-467d-883c-bff55819e867",
    "title": "Queremos ouvir a sua opnião",
    "description": "De 0 a 10 quanto você recomendaria a Rocketseat?",
    "created_at": "2021-02-27T20:37:57.000Z"
  }
]
```
### GET
/nps/:id_surveys

```
{
  "detractor": 1,
  "promoters": 2,
  "passive": 0,
  "totalAnswers": 3,
  "nps": 33.33
}
```

## Resultado final:

Após clicar em uma nota

value = nota enviada
```
{
"id": "276349db-62e1-4a65-b472-f826c0af86f6",
"user_id": "33fce935-8ff5-4e73-8b1e-71ad3355b9a9",
"survey_id": "f101a328-8fd4-431b-9b3d-78ecf56a2f1a",
"value": 1,
"created_at": "2021-02-27T18:26:03.000Z"
}

```

<img src="https://github.com/Strongreen/NLW4-Rocketseat-Fevereiro/blob/main/resultado_final.png" alt="imagem do projeto final"/>




