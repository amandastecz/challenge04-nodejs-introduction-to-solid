# Introdução ao SOLID

Essa será uma aplicação de listagem e cadastro de usuários. Para que a listagem de usuários funcione, o usuário que solicita a listagem deve ser um admin (mais detalhes ao longo da descrição).

## Controllers e Use Cases:

### POST `/users`

-[X] A rota deve receber `name`, e `email` dentro do corpo da requisição para que seja possível cadastrar um usuário.

### PATCH `/users/:user_id/admin`

-[X] A rota deve receber, nos parâmetros da rota, o `id` de um usuário e transformar esse usuário em admin.

### GET `/users/:user_id`

-[X] A rota deve receber, nos parâmetros da rota, o `id` de um usuário e devolver as informações do usuário encontrado pelo corpo da resposta.

### GET `/users`

-[X] A rota deve receber, pelo header da requisição, uma propriedade `user_id` contendo o `id` do usuário e retornar uma lista com todos os usuários cadastrados. O `id` deverá ser usado para validar se o usuário que está solicitando a listagem é um admin. O retorno da lista deve ser feito apenas se o usuário for admin.

## Models
-[X] Criar model do user

## Repository
-[X] Implementar lógica do create user
-[X] Implementar lógica para listar todos os usuários
-[X] Implementar lógica para encontrar um user pelo id
-[X] Implementar lógica para encontrar um user pelo e-mail
-[X] Implementar lógica para tornar um usuário como admin

## Documentação
- Acesse a documentação em http://localhost:3333/api-docs/#/
