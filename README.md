
<h1 align="center">
 Kenzie Burguer
</h1>

<p align = "center">
    Este é o Backend da Aplicação do burguers, uma hamburgueria
</p>

<p align="center">
  <a href="#endpoints">Endpoints</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</p>


## **Endpoints**

A API no momento possui 5 endpoints sendo elas de Login, Cadastro, Feedbacks, Produtos, ver Feedbacks

O URL base da aplicação é https://hamburgueria-api-kenzie-academ.herokuapp.com/


# Rotas da Aplicação


<h2 align="center">Login</h2>

<p align="center">Post /login</p>

<h4 align="center">Formato da Requisição:</h4>

```Post /login
{
	"email": "kenzinho@gmail.com",
	"password": "123456"
}
```

<h4 align="center">Resposta:<h4>
```
{
  "accessToken": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6IndhbGxhY2VzZm9zQGhvdG1haWwuY29tIiwiaWF0IjoxNjM1Mjk5ODExLCJleHAiOjE2MzUzMDM0MTEsInN1YiI6IjIifQ.b4fGy1IhMhm2CSzEFtBS8XQEcOCKxY1EbLL-K3rD0aw",
  "user": {
    "email": "kenzinhoo@gmail.com",
    "name": "kenzinho",
    "age": 25,
    "id": 4
  }
}
```

<h2 align="center">Registro</h2>

<p align="center">Post /register</p>

<h4 align="center">Formato da Requisição:</h4>

```json
    {
        "email": "kenzinho@gmail.com",
        "password": "123456",
        "name": "kenzinho",
        "age": 25
    }
```


<h4 align="center">Resposta:<h4>
	
```
  {
  "accessToken": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6Imtlbnppbmhvb0BnbWFpbC5jb20iLCJpYXQiOjE2MzUyOTk5NTEsImV4cCI6MTYzNTMwMzU1MSwic3ViIjoiNCJ9.2IQjXtcmQV6VEqzxwwB6zNnJs5WrUwmflovFQRJF92U",
  "user": {
    "email": "kenzinhoo@gmail.com",
    "name": "kenzinho",
    "age": 25,
    "id": 4
  }
}
```
<h2>Produtos</h2>

<p align="center">GET /produtos</p>

<h4 align="center">Formato da Requisição:</h4>

```
GET /products
```

<h4 align="center">Resposta:</h4>
	
```
{
      {
    "name": "Big Kenzie",
    "description": "Não existe nada igual. Dois hambúrgueres, alface, queijo e molho especial, cebola e picles num pão com gergelim.",
    "price": 15,
    "image": "https://cache-backend-mcd.mcdonaldscupones.com/media/image/product$kfXxD5Xb/200/200/original?country=br",
    "category": "hamburguer"
    },
      [...]
```


<h2>Feedback</h2>

<p align="center">post /feedbacks</p>

<h4 align="center">Formato da Requisição:</h4>

```
Post /feedbacks

{
	"name": "kenzinho",
	"feedback": "text... ",
	"userId": 2 (Aqui entra o ID do seu usuário)
}
```
<p align="center">Essa requisição só irá funcionar se você estiver logado</p>

<h4 align="center">Resposta:</h4>

```
{
  "name": "kenzinho",
  "feedback": "text....",
  "userId": 2,
  "id": 2
}
```

