# Casos de Teste

## Caso 1 (Passo a Passo): Login com Sucesso
1. Acessar o site https://www.saucedemo.com/
2. No campo "Username", digitar "standard_user"
3. No campo "Password", digitar "secret_sauce"
4. Clicar no botão "Login"
**Resultado Esperado:** O usuário deve ser redirecionado para a página de produtos (Inventory).

## Caso 2 (Passo a Passo): Login com Senha Incorreta
1. Acessar o site https://www.saucedemo.com/
2. No campo "Username", digitar "standard_user"
3. No campo "Password", digitar "senha_errada"
4. Clicar no botão "Login"
**Resultado Esperado:** O sistema deve exibir a mensagem de erro "Epic sadface: Username and password do not match any user in this service".

## Caso 3 (BDD): Adicionar Mochila ao Carrinho
**Dado** que estou logado na loja SwagLabs
**Quando** eu clico no botão "Add to cart" do produto "Sauce Labs Backpack"
**Então** o botão deve mudar o texto para "Remove"
**E** o contador do carrinho deve exibir "1"

## Caso 4 (BDD): Remover Produto do Carrinho
**Dado** que tenho a "Sauce Labs Backpack" no meu carrinho
**Quando** eu clico no botão "Remove"
**Então** o botão deve voltar a exibir "Add to cart"
**E** o contador do carrinho deve ficar vazio
