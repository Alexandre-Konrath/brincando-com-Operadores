## Selecionando atributos e (campos)

- Neste primeiro estou apenas unando o `.findAll()` que me retorna todos os customers.
   
![1](https://github.com/Alexandre-Konrath/Brincando-com-Operadores/assets/160286787/aedd92bc-713c-462b-a752-4bdaa26f4c6c)
##

- Já neste estou usando o `attributes: []`, ira retornar todos pelo uso do `.findAll()` porem somente mostrando o "id" e o "name".

![2](https://github.com/Alexandre-Konrath/Brincando-com-Operadores/assets/160286787/4ac9ef75-bc92-42d0-a1b8-d3561fba7de6)                        

 - E neste uso o `exclude: [ ]`, que irá buscar e exibir todos com a exceção do "status" e "id".
![3](https://github.com/Alexandre-Konrath/Brincando-com-Operadores/assets/160286787/13e0c814-1d86-4a68-b073-9b5f20d7a922)
##

- Usando o `limit: 1` ele exibe somente o primeiro customer, mesmo usnado o `.findAll()`.
![4](https://github.com/Alexandre-Konrath/Brincando-com-Operadores/assets/160286787/86ca7159-39f9-4f27-a246-982048f8cf9d)

- Usando o `.findOne()` retorna somente o primeiro apenas.
![5](https://github.com/Alexandre-Konrath/Brincando-com-Operadores/assets/160286787/08eda1c6-d40a-4948-bddc-d9df7d1c7398)

- E Usando o `.findByPk(1)` retorna o customer com o id 1.
![6](https://github.com/Alexandre-Konrath/Brincando-com-Operadores/assets/160286787/f6cf0722-c8ed-4c0f-8941-5f47acd8ea2e)
##

## filtros (where)
- Usando o `where: {}` para buscar pelo id, ele me retorna corretamete o customer com id 1, unico problema é que ele aida é um array.
![7](https://github.com/Alexandre-Konrath/Brincando-com-Operadores/assets/160286787/77b3e498-34f6-4625-8937-b26c7e6ae607)

mas para resolver isso é só usar o `.findOne()`.
![8](https://github.com/Alexandre-Konrath/Brincando-com-Operadores/assets/160286787/90630ff1-feba-461d-9fd5-727a0249eb7b)

- E nesse estou filtrando somente para os customers ACTIVE. Mas o interessante é que ele mostra pra gente todo o comando sql que esta sendo usado .
![9](https://github.com/Alexandre-Konrath/Brincando-com-Operadores/assets/160286787/0e7cf1ec-2be7-4861-b01d-22d797840d22)

- Com os Operadores tem mais opções de filtro com o `[Op.eq]` que me retorna somente os "ACTIVE".

![10](https://github.com/Alexandre-Konrath/Brincando-com-Operadores/assets/160286787/c6689e84-5a5f-4829-9ba7-3cc9c0d86b18)               
e o `[Op.ne]` retorna o contrario de "ACTIVE".
![11](https://github.com/Alexandre-Konrath/Brincando-com-Operadores/assets/160286787/04df77ab-e831-404c-9fb3-a9f3244a45d7)

e usando o `[Op.in]` ele aceita array.
![12](https://github.com/Alexandre-Konrath/Brincando-com-Operadores/assets/160286787/c1a98b07-9cb6-4048-9c53-a6ebe07c4b1b)

- Com o `[Op.like]` ele filtra pelo nome.

![13](https://github.com/Alexandre-Konrath/Brincando-com-Operadores/assets/160286787/e470c7b5-011c-4c7f-99c1-324548013667)

- E com o `[Op.between]` fazendo o filtro com datas, neste caso ele retorna todos porem o interessante é ver o sql usando o BETWEN e o AND, fiz uma mudaça pra filtrar os ids com ordem crescente.

![14](https://github.com/Alexandre-Konrath/Brincando-com-Operadores/assets/160286787/d9d25abf-6f7c-4573-80da-4bce14d37cdf)



