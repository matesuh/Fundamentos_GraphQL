Fundamentos GraphQL na prática (Node.js + React)

- Quais problemas GraphQL resolve?
    - Overfetching
        - http://localhost:3000/users
        - DB (usuários, endereços)
    - Underfetching
        - http://localhost:3000/users
        - DB (usuário)
    - http://localhost:3000/addresses
- http://localhost:3000/graphql

Dificuldades:

- Cache
- Erros

```gql
query {
	users {
		id
		name
		github

		addresses {
			city
			state
			country
		}
	}
}
```