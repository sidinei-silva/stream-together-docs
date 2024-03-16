# Caso de uso: Editar compartilhamento

## **Descrição**

Este caso de uso permite que o usuário edit um compartilhamento de streaming.

## **Atores**

- Usuário
- Sistema

## **Entradas**

- ID do compartilhamento
- Dados do compartilhamento
  - Nome
  - Valor mensalidade
  - Vencimento
  - Quantidade de membros
  - Email de entrada no streaming
  - Senha de entrada no streaming
  - Status

## **Pré-condições**

- Usuário autenticado
- Compartilhamento existe
- Usuário é o criador do compartilhamento

## **Regras de negócio**

- O compartilhamento deve existir
- O usuário deve ser o criador do compartilhamento
- O sistema deve exibir mensagem de erro se o compartilhamento não existir
- O sistema deve exibir mensagem de erro se o usuário não for o criador do compartilhamento
- A quantidade total de membros deve ser maior ou igual a quantidade de membros atual
- O valor da mensalidade deve ser maior que zero

## **Fluxo principal**

1. O caso de uso se inicia quando o usuário clica no botão "Editar compartilhamento".
2. O sistema valida se o usuário é o criador do compartilhamento.
3. O sistema exibe o formulário de edição do compartilhamento.
4. O usuário preenche os campos do formulário.
5. O usuário clica no botão "Salvar".
6. O sistema valida os dados do formulário.
7. O sistema atualiza os dados do compartilhamento.
8. O caso de uso é encerrado.

## **Fluxo alternativo**

### **Compartilhamento não existe**

1. O sistema exibe uma mensagem de erro informando que o compartilhamento não existe.
2. O caso de uso é encerrado.

### **Usuário não é o criador do compartilhamento**

1. O sistema exibe uma mensagem de erro informando que o usuário não é o criador do compartilhamento.
2. O caso de uso é encerrado.

### **Dados inválidos**

1. O sistema exibe uma mensagem de erro informando que os dados do formulário são inválidos.
2. O caso de uso é encerrado.

## **Pós-condições**

- O compartilhamento é editado.
- O valor da mensalidade por membro é atualizado.
