![logo](https://itzone.com.vn/wp-content/uploads/2020/04/Symfony.jpg)

## Symfony also is useful with API
Identify how create APIs in Symfony, creating and reading post and only reading categories

## Tech Stack
**Server:** [Symfony 6](https://symfony.com/), [API Platform](https://api-platform.com/)

## Installation
1. Clone this repository.
2. Navegate to the project directory
3. Run `composer install` to install the dependencies.
4. Configure your environment variables.

## API Reference

### Category
| Type | Path |Description| Params   
|:-|:-|:-|:-
| `GET` | `/api/categories`|All categories|

```json
{
  "id": 0,
  "name": "string",
  "posts": [
    "string"
  ]
}
```

| Type | Path |Description| Params   
|:-|:-|:-|:-
| `GET` | `/api/categories/{id}`|Category id|An specific category|
```json
{
  "id": 0,
  "name": "string",
  "posts": [
    "string"
  ]
}
```
##
### Post
| Type | Path |Description| Params   
|:-|:-|:-|:-
| `GET` | `/api/posts`|All posts|
```json
{
    "id": 0,
    "title": "string",
    "category": {
      "id": 0,
      "name": "string"
    },
    "summary": "string"
  }
```

| Type | Path |Description| Params   
|:-|:-|:-|:-|
| `GET` | `/api/posts/{id}`|Post id|An specific post| id
```json
{
  "id": 0,
  "title": "string",
  "body": "string",
  "category": {
    "id": 0,
    "name": "string"
  }
}
```

| Type | Path |Description| Params   
|:-|:-|:-|:-
| `POST` | `/api/posts`|Create a post| title, body, category
```json
{
  "id": 0,
  "title": "string",
  "body": "string",
  "category": "string",
  "summary": "string"
}
```

| Type | Path |Description| Params   
|:-|:-|:-|:-
| `PATCH` | `/api/posts/{id}`|Update a post| id, title, body, category
```json
{
  "id": 0,
  "title": "string",
  "body": "string",
  "category": "string",
  "summary": "string"
}
```

## Links

[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://angelprz8a.github.io/Portafolio/)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/angelprz8a/)

## License
The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).

