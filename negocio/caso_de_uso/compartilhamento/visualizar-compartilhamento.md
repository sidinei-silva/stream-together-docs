# Caso de uso: Visualizar compartilhamento de streaming

## **Descrição**

Este caso de uso descreve como um usuário pode visualizar um compartilhamento de contas de streaming.

## **Atores**

- Usuário

## **Entradas**

- Identificador do compartilhamento

## **Pré-condições**

- Usuário autenticado
- Compartilhamento existe
- Usuário possui permissão para visualizar o compartilhamento

## **Regras de negócio**

- O compartilhamento deve existir
- O usuário deve ser membro do compartilhamento
- Somente membros do compartilhamento podem visualizá-lo
- Sistema deve exibir mensagem de erro se o compartilhamento não existir
- Sistema deve exibir mensagem de erro se o usuário não possuir permissão para visualizar o compartilhamento

## **Fluxo principal**

1. O caso de uso se inicia quando o usuário clica no botão "Visualizar compartilhamento".
2. O sistema valida se o usuário possui permissão para visualizar o compartilhamento.
3. O sistema exibe a página do compartilhamento.
4. O caso de uso é encerrado.

## **Fluxo alternativo**

### **Compartilhamento não existe**

1. O sistema exibe uma mensagem de erro informando que o compartilhamento não existe.
2. O caso de uso é encerrado.

### **Usuário não possui permissão para visualizar o compartilhamento**

1. O sistema exibe uma mensagem de erro informando que o usuário não possui permissão para visualizar o compartilhamento.
2. O caso de uso é encerrado.

## **Pós-condições**

- O usuário visualiza o compartilhamento de streaming.
- O caso de uso é encerrado.
