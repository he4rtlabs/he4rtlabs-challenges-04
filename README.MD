# Projeto 004 - Try Catch 'Em all 

Pokedéx boladona pra você pegar todos os pokemões do planeta (que você cadastrar)

## Qual é o valor que o desafio entrega?

O projeto tem a finalidade de descrever alguns fatores determinantes para você melhorar sua ideia de banco de dados relacional, consumo de API's e integração.

1. Relações Pertencem à Muitos (BelongsToMany)

    Quando você tem duas tabelas e você quer relacionalas com duas chaves "primárias", você usa a relação BelongsToMany.

2. Consumo de API de terceiros

   Você irá fazer uma classe (Service) para consumir a API do [PokeApi.co](https://pokeapi.co) e aprender sobre CURL.

3. Projeto Fullstack

    Deverá ser uma aplicação com Front e Back-end, onde você deverá julgar como separar essa arquitetura.

### Desafio

Faça uma aplicação (com ou sem autenticação) onde você poderá ter um registro global de pokémons, pegando dados da PokeApi para popular seu banco.

A ideia é você poder cadastrar treinadores e nesses treinadores você deverá vincular pokémons nos quais você quiser.

Modelo de tabelas sugerido: 

```
table: trainers
------
id: int primary key auto increment
name: string
region: string (Kanto, Johto, Hoenn, Sinnoh)
age: int


table: pokemons
------
id: int primary key auto increment
name: string
image_url: string 
attribute: string (lighning, ice, fire etc)

table: trainer_pokemons
------
trainer_id: int references id in trainers
pokemon_id int references id in pokemons
```

Cuidados a se tomar:

- Fazer um layout agradável e o plus de algo tematizado;
- Não ter pressa para terminar o projeto.

### Conclusão do Desafio

Commite as alterações feitas e faça um post ou no nosso Discord na sala #he4rtlabs-challenges ou um post no Twitter com a hashtag #He4rtLabsChallenges e iremos divulgar e/ou fazer um review do seu código.

Caso você se sinta confortável, deixamos um arquivo chamado REVIEW.MD para você fazer alguns comentários sobre o desafio e o que você achou no geral.

## Créditos

Este desafio foi desenvolvido pelo grupo He4rt Developers para uso livre da comunidade.

## Autor

- Daniel Reis (danielhe4rt) - Back-end Developer && He4rt Developers Leader - [Portfólio](https://danielheart.dev) - [Twitter](https://twitter.com/danielhe4rt)
