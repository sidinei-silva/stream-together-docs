# Caso de uso: Remover membro no compartilhamento

## **Descrição**

Este caso de uso descreve como um usuário pode remover um membro de um compartilhamento de contas de streaming.

## **Atores**

- Usuário
- Sistema
- Membro

## **Entradas**

- ID do compartilhamento
- ID do membro

## **Pré-condições**

- Usuário autenticado
- Compartilhamento existe
- Usuário é o criador do compartilhamento
- Usuário é membro do compartilhamento

## **Regras de negócio**

- O compartilhamento deve existir
- O usuário deve ser o criador do compartilhamento
- O usuário deve ser membro do compartilhamento
- O sistema deve exibir mensagem de erro se o compartilhamento não existir
- O sistema deve exibir mensagem de erro se o usuário não for o criador do compartilhamento
- O sistema deve exibir mensagem de erro se o usuário não for membro do compartilhamento
- O sistema deve exibir mensagem de erro se o membro não existir
- O sistema deve exibir mensagem de erro se o usuário tentar remover a si mesmo do compartilhamento

## **Fluxo principal**

1. O caso de uso se inicia quando o usuário clica no botão "Remover membro".
2. O sistema valida se o usuário é o criador do compartilhamento.
3. O sistema exibe uma lista de membros do compartilhamento.
4. O usuário seleciona o membro que deseja remover.
5. O sistema exibe um modal de confirmação.
6. O usuário confirma a remoção.
7. O sistema remove o membro do compartilhamento.
8. O sistema exibe uma mensagem de sucesso.
9. O sistema recalcula o valor da mensalidade do compartilhamento.
10. O caso de uso é encerrado.

## **Fluxo alternativo**

### **Membro não existe**

1. No passo 4 do fluxo principal, o sistema exibe uma mensagem de erro informando que o membro não existe.
2. O caso de uso é encerrado.

### **Usuário não é o criador do compartilhamento**

1. No passo 2 do fluxo principal, o sistema exibe uma mensagem de erro informando que o usuário não é o criador do compartilhamento.
2. O caso de uso é encerrado.

### **Usuário não é membro do compartilhamento**

1. No passo 2 do fluxo principal, o sistema exibe uma mensagem de erro informando que o usuário não é membro do compartilhamento.
2. O caso de uso é encerrado.

### **Usuário tenta remover a si mesmo do compartilhamento**

1. No passo 6 do fluxo principal, o sistema exibe uma mensagem de erro informando que o usuário não pode remover a si mesmo do compartilhamento.
2. O caso de uso é encerrado.

### **Cancelamento da remoção**

1. No passo 6 do fluxo principal, o usuário cancela a remoção.
2. O caso de uso é encerrado.

## **Pós-condições**

- Membro removido do compartilhamento
- Mensalidade recalculada
- Mensagem de sucesso exibida
