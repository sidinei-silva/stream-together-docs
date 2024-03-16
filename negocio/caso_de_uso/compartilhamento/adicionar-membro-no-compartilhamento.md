# Caso de uso: Adicionar membro no compartilhamento

## **Descrição**

Este caso de uso descreve como um usuário pode adicionar um membro em um compartilhamento de contas de streaming.

## **Atores**

- Usuário
- Sistema
- Membro

## **Entradas**

- ID do compartilhamento
- Email do membro

## **Pré-condições**

- Usuário autenticado
- Compartilhamento existe
- Usuário é o criador do compartilhamento
- Usuário não é o membro do compartilhamento
- Existe cadastro do membro com o email informado

## **Regras de negócio**

- O compartilhamento deve existir
- O usuário deve ser o criador do compartilhamento
- O usuário não pode ser membro do compartilhamento
- O membro deve existir
- O sistema deve exibir mensagem de erro se o compartilhamento não existir
- O sistema deve exibir mensagem de erro se o usuário não for o criador do compartilhamento
- O sistema deve exibir mensagem de erro se o usuário já for membro do compartilhamento
- O sistema deve exibir mensagem de erro se o membro não existir
- O compartilhamento deve ter vagas disponíveis

## **Fluxo principal**

1. O caso de uso se inicia quando o usuário clica no botão "Adicionar membro".
2. O sistema valida se o usuário é o criador do compartilhamento.
3. O sistema valida se o compartilhamento tem vagas disponíveis.
4. O sistema exibe um formulário para preenchimento do email do membro.
5. O usuário preenche o campo do formulário e clica no botão "Adicionar".
6. O sistema valida os dados do formulário.
7. O sistema valida se usuário existe.
8. O sistema verifica se o usuário já é membro do compartilhamento.
9. O sistema adiciona o membro no compartilhamento.
10. O sistema exibe uma mensagem de sucesso.
11. O caso de uso é encerrado.

## **Fluxo alternativo**

### **Compartilhamento não existe**

1. O sistema exibe uma mensagem de erro informando que o compartilhamento não existe.
2. O caso de uso é encerrado.

### **Usuário não é o criador do compartilhamento**

1. O sistema exibe uma mensagem de erro informando que o usuário não é o criador do compartilhamento.
2. O caso de uso é encerrado.

### **Usuário já é membro do compartilhamento**

1. O sistema exibe uma mensagem de erro informando que o usuário já é membro do compartilhamento.
2. O caso de uso é encerrado.

### **Usuário não existe**

1. O sistema exibe uma mensagem de erro informando que o usuário não existe.
2. O caso de uso é encerrado.

### **Compartilhamento não tem vagas disponíveis**

1. O sistema exibe uma mensagem de erro informando que o compartilhamento não tem vagas disponíveis.
2. O caso de uso é encerrado.

## **Pós-condições**

- Membro adicionado no compartilhamento
- O caso de uso é encerrado.
