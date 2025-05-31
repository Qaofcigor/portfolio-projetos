# Ambiente de Teste Automatizado de API

Este projeto está configurado para realizar testes automatizados de API utilizando Postman e Newman.

## Como usar

1. Instale as dependências:
   ```
   npm install
   ```

2. Execute os testes:
   ```
   npm test
   ```

   Isso executará a coleção de exemplo `collection-sample.json` usando o Newman e mostrará os resultados no terminal.

## Personalização

- Para adicionar suas próprias coleções do Postman, coloque os arquivos JSON na raiz do projeto.
- Atualize o script `test` no `package.json` para apontar para sua coleção, por exemplo:
  ```json
  "scripts": {
    "test": "newman run sua-colecao.json"
  }
  ```
- Exemplos adicionais de coleções incluídas neste projeto:
  - `collection-post-example.json`: Exemplo de requisição POST com testes de status e conteúdo.
  - `collection-put-example.json`: Exemplo de requisição PUT com testes de atualização.
  - `collection-delete-example.json`: Exemplo de requisição DELETE com teste de status.

## Requisitos

- Node.js e npm instalados na sua máquina.
- Newman instalado como dependência do projeto (já configurado).

## Referências

- [Postman](https://www.postman.com/)
- [Newman](https://www.npmjs.com/package/newman)

Este ambiente está pronto para você começar a estudar e automatizar testes de API.
