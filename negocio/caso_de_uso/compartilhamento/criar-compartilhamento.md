# Caso de uso: Criar compartilhamento de streamimg

## **Descrição**

Este caso de uso descreve como um usuário pode criar um compartilhamento de contas de streaming.

## **Atores**

- Usuário
- Sistema

## **Entradas**

- Nome do serviço de streaming
- Valor total da mensalidade
- Número de vagas disponíveis
- Email de entrada no streaming
- Senha de entrada no streaming
- Data de vencimento

## **Pré-condições**

- Usuário autenticado
- Usuário não possui compartilhamento com o mesmo serviço de streaming

## **Regras de negócio**

- O valor total da mensalidade deve ser maior que zero.
- O número de vagas disponíveis deve ser maior que zero.
- A data de vencimento deve ser maior que a data atual.
- O usuário não pode criar um compartilhamento com o mesmo nome de serviço de streaming.

## **Fluxo principal**

1. O caso de uso se inicia quando o usuário clica no botão "Criar compartilhamento".
2. O sistema exibe um formulário para preenchimento dos dados do compartilhamento.
3. O usuário preenche os campos do formulário e clica no botão "Criar".
4. O sistema valida os dados do formulário.
5. O sistema valida se o usuário já possui um compartilhamento com o mesmo nome de serviço de streaming.
6. O sistema cria o compartilhamento.
7. O sistema exibe uma mensagem de sucesso.
8. O sistema redireciona o usuário para a página do compartilhamento.
9. O caso de uso é encerrado.

## **Fluxo alternativo**

### **Compartilhamento já existe**

1. No passo 5 do fluxo principal, o sistema identifica que o usuário já possui um compartilhamento com o mesmo nome de serviço de streaming.
2. O sistema exibe uma mensagem de erro.
3. O caso de uso é encerrado.

### **Erro de validação**

1. No passo 4 do fluxo principal, o sistema identifica que os dados do formulário são inválidos.
2. O sistema exibe uma mensagem de erro.
3. O caso de uso é encerrado.

## **Pós-condições**

- Compartilhamento criado
- Mensagem de erro
- Usuário redirecionado para a página do compartilhamento
