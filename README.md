# Secure Register

Secure Register é uma aplicação Spring Boot que permite o registro e autenticação de usuários. A aplicação utiliza Spring Security para gerenciar a segurança e autenticação dos usuários.

## Funcionalidades

- Registro de novos usuários.
- Autenticação de usuários existentes.
- Listagem de todos os usuários cadastrados.

## Endpoints

### 1. Registrar Usuário

**Endpoint:** `POST http://localhost:8080/auth/register`

**Corpo da Requisição:**
```json
{
    "username": "vinicius",
    "password": "Senha123"
}

**GET http://localhost:8080/auth/login**

username: Nome de usuário
password: Senha

http://localhost:8080/auth/login?username=vinicius&password=Senha123
Usuário autenticado com sucesso!


GET http://localhost:8080/auth/users

[
  {
    "id": 1,
    "username": "vini",
    "password": "$2a$10$odPjh9Ox0eL.qv9EaTMi/OD5zXOovAfhG4ubmrikqXZZkZcegWWJe",
    "enabled": true,
    "credentialsNonExpired": true,
    "accountNonExpired": true,
    "accountNonLocked": true,
    "authorities": []
  },
  {
    "id": 2,
    "username": "vini2",
    "password": "$2a$10$YZjmkNl/2r8kCe4u6AQJaewHl.NNp2sXWRVC329CelJFk1U9DrvG6",
    "enabled": true,
    "credentialsNonExpired": true,
    "accountNonExpired": true,
    "accountNonLocked": true,
    "authorities": []
  },
  {
    "id": 3,
    "username": "vini3",
    "password": "$2a$10$tKLxFLYoDtfhDlFzTdYHfe4j1Gx5iHIL2HIflziM8sA7i5oEqGdM.",
    "enabled": true,
    "credentialsNonExpired": true,
    "accountNonExpired": true,
    "accountNonLocked": true,
    "authorities": []
  }
]

