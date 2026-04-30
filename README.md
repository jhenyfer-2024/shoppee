Esse código foi feito pra simular um carrinho de compras simples, tipo de loja online.

No início eu importei as funções do carrinho (cartService) e também uma função chamada createItem, que é responsável por criar os produtos. Depois disso, criei duas listas: uma pro carrinho (myCart) e outra pra lista de desejos (myWhishList), mas a de desejos ainda não está sendo usada.

Coloquei uma mensagem no console só pra dar uma introdução quando o código roda.

Em seguida, criei dois itens passando nome, preço e quantidade. Usei como exemplo dois carrinhos Hot Wheels, um Ferrari e um Lamborghini.

Depois de criar os itens, adicionei os dois no carrinho usando a função addItem. Em seguida, usei a função removeItem várias vezes no mesmo produto pra testar o comportamento: primeiro ele vai diminuindo a quantidade, e quando chega em 1, ele remove o item completamente do carrinho.

No final, usei displaycart pra mostrar todos os itens que ficaram no carrinho e calculateTotal pra somar o valor total.

As funções do carrinho foram separadas em outro arquivo pra organizar melhor o código.

A função addItem só adiciona um item no array do carrinho usando push.

A função calculateTotal percorre todos os itens do carrinho usando reduce e soma os subtotais, mostrando o valor final no console.

A função deleteItem remove um item direto pelo nome. Ela procura o índice com findIndex e, se encontrar, usa splice pra remover.

A função removeItem é um pouco mais completa: ela procura o item, e se não encontrar mostra uma mensagem. Se encontrar e a quantidade for maior que 1, ela diminui 1 unidade. Se a quantidade for igual a 1, ela remove o item do carrinho.

Por fim, a função displaycart lista todos os produtos do carrinho, mostrando nome, preço, quantidade e o subtotal de cada item.

No geral, é um sistema básico de carrinho que consegue adicionar, remover, listar produtos e calcular o total, simulando a lógica principal de um e-commerce.
