# CrudStarWars - API

Projeto utilizando Spring Boot, e MongoDB.

## O problema

Desenvolver uma API que contenha os dados dos planetas da galáxia distante de Star Wars.
* A API deve ser REST
*  Para cada planeta, os seguintes dados devem ser obtidos do banco de dados
da aplicação, sendo inseridos manualmente: Nome Clima Terreno
* Para cada planeta também devemos ter a quantidade de aparições em filmes,
que podem ser obtidas pela API pública do Star Wars: https://swapi.co/
* A API deverá conseguir adicionar um planeta (com nome, clima e terreno),
listar planetas, buscar por nome, buscar por ID, remover planeta

Tecnologias a serem utilizadas:
* Spring Boot
* Java 8
* MongoDB (pode-se utilizar o Spring Data)
* Aconselha-se utilizar JPA

Funções necessárias:
* Consumir do https://swapi.co/
	* Quando um planeta é salvo, há a comunicação com o site, que obtém o número de aparições
* Obter os planetas inseridos (GET)
* Incluir planeta (POST - formato JSON)
* Buscar planeta pelo **nome** (GET)
* Buscar planeta por **id** (GET)
* Remover um planeta (por **id** - DELETE)

## Rotas
| Requisição| Path | Função |
|--|--|--|
| GET | /api/planetas | Lista todos os planetas
|POST| /api/planetas| Cria um planeta
|PUT| /api/planetas/id/{id}| Atualiza um planeta
|DELETE| /api/planetas/id/{id}| Remove um planeta
|GET| /api/planetas/id/{id}| Busca um planeta por ID
|GET| /api/planetas/nome/{nome}| Busca um planeta por nome
