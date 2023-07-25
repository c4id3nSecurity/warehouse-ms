# Warehouse-ms

## Endpoints
- BaseURL: /warehouse
- POST: create()
- GET: getAll()
- GET: /{id}: getById()
- DELETE: /{id}: delete()

## Model
```json
{
  "id": 1,
  "productId": 1,
  "quantity": 10
}
```

## Business Rules
- O estoque é responsável por avisar se o produto está ou não disponivel. Ou seja caso o valor da quantidade seja igual a 0, deve informar outro serviço;
- Não é permitido mais de uma linha do mesmo produto salvo na base de dados;