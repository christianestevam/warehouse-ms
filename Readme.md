## Warehouse-ms

- BaseUrl: /warehouses
- POST: create()
- GET: getAll()
- GET /{id}: getByid()"
- PUT /{id}: update()


## Model
```json
{
	"id": 1,
	"product-id": 13,
	"quantity": 10,
	"isAvailable": true
}


## Business Rules
- O estoque é responsável por avisa se o produto está ou não disponivel. Ou seja caso a quantidade do produto for igual a 0 deve avisar o outro serviço;
- Não é permitido mais de uma linha do mesmo produto salvo na base de dados;
