# Documentação da API - Coleções de Teste

Este documento descreve as coleções de testes de API configuradas no projeto para facilitar o entendimento e uso.

## 1. Sample API Test Collection (GET)

- Endpoint: `GET https://jsonplaceholder.typicode.com/posts/1`
- Descrição: Requisição simples para obter um post pelo ID.
- Testes:
  - Verifica se a resposta retorna status 200 OK.

## 2. POST Request Example

- Endpoint: `POST https://jsonplaceholder.typicode.com/posts`
- Descrição: Cria um novo post com título, corpo e userId.
- Corpo da requisição (JSON):
  ```json
  {
    "title": "foo",
    "body": "bar",
    "userId": 1
  }
  ```
- Testes:
  - Verifica se o status da resposta é 201 Created.
  - Verifica se a resposta contém a propriedade `id`.

## 3. PUT Request Example

- Endpoint: `PUT https://jsonplaceholder.typicode.com/posts/1`
- Descrição: Atualiza o post com ID 1.
- Corpo da requisição (JSON):
  ```json
  {
    "id": 1,
    "title": "foo updated",
    "body": "bar updated",
    "userId": 1
  }
  ```
- Testes:
  - Verifica se o status da resposta é 200 OK.
  - Verifica se o título da resposta foi atualizado.

## 4. DELETE Request Example

- Endpoint: `DELETE https://jsonplaceholder.typicode.com/posts/1`
- Descrição: Deleta o post com ID 1.
- Testes:
  - Verifica se o status da resposta é 200 OK ou 204 No Content.

---

Esta documentação serve como referência para os testes automatizados configurados no projeto usando Postman e Newman.
