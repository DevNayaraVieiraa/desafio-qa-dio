# Mapa Mental de Testes - Login SwagLabs

- **Funcionalidade: Login**
    - **Cenário: Sucesso**
        - Usuário: standard_user
        - Senha: secret_sauce
        - Resultado: Acesso à Home
    - **Cenário: Falha**
        - **Usuário Bloqueado**
            - Usuário: locked_out_user
            - Resultado: Mensagem "Sorry, this user has been locked out"
        - **Dados Incorretos**
            - Senha errada
            - Usuário inexistente
            - Resultado: Mensagem "Username and password do not match"
    - **Elementos da Tela**
        - Campo Username
        - Campo Password
        - Botão Login
