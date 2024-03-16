# Caso de uso: Resetar senha do usuário

## **Descrição**

Este caso de uso descreve o processo de resetar a senha do usuário.

## **Atores**

- Usuário

## **Entradas**

- E-mail: Email do usuário

## **Saídas**

- E-mail de confirmação de reset de senha
- Confirmação de reset de senha
- Mensagem de erro
  - E-mail não cadastrado

## **Pré-condições**

- Usuário deve estar cadastrado na plataforma
- Usuário deve ter acesso ao e-mail cadastrado

## **Fluxo principal**

1. O Usuário insere seu e-mail.
2. O sistema envia um e-mail com um link para resetar a senha com um token de validação.
3. O Usuário clica no link do e-mail.
4. O sistema valida o token.
5. O sistema redireciona o usuário para a página de reset de senha.
6. O Usuário insere a nova senha.
7. O sistema valida a nova senha.
8. O sistema confirma o reset de senha.
9. O sistema redireciona o usuário para a página de login.
10. Fim do caso de uso.

## **Fluxo alternativo**

### **E-mail não cadastrado**

1. O sistema informa que o e-mail inserido não está cadastrado.
2. Fim do caso de uso.

### **Token inválido:**

1. O sistema informa que o token inserido é inválido.
2. Fim do caso de uso.

### **Senha não confere:**

1. O sistema informa que a senha inserida não confere com a confirmação.
2. Fim do caso de uso.

## **Pós-condições**

- Usuário deve receber um e-mail de confirmação de reset de senha.
- Usuário deve conseguir trocar a senha.
