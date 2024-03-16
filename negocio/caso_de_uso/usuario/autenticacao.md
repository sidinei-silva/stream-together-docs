# Autenticação de Usuário

## **Atores:**

- Usuário

## **Entradas:**

- E-mail: Email do usuário
- Senha: Senha do usuário

## **Saídas:**

- Acesso a plataforma
- Mensagem de erro
  - E-mail ou senha inválidos
  - Usuário não cadastrado

## **Pré-condições:**

- Usuário deve estar cadastrado na plataforma

## **Fluxo Principal:**

1. O Usuário insere suas credenciais de login: e-mail e senha.
2. O sistema valida as credenciais.
3. O sistema concede acesso ao dashboard do usuário.
4. Fim do caso de uso.

## **Fluxos Alternativos:**

- **E-mail ou senha inválidos:**
  1. O sistema informa que as credenciais inseridas são inválidas.
  2. Fim do caso de uso.
- **Usuário não cadastrado:**
  1. O sistema informa que o usuário não está cadastrado.
  2. Fim do caso de uso.
