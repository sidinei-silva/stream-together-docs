# Caso de uso: Listar compartilhamentos de streaming

## **Descrição**

Este caso de uso descreve como um usuário pode listar os compartilhamentos de contas de streaming.

## **Atores**

- Usuário
- Sistema

## **Entradas**

- Nenhuma

## **Pré-condições**

- Usuário autenticado
- Usuário possui compartilhamentos ou ser membro de compartilhamentos

## **Regras de negócio**

- O sistema deve exibir a lista de compartilhamentos do usuário
- O sistema deve exibir compartilhamentos dos quais o usuário é membro
- O sistema deve dar opção de visualizar os compartilhamentos
- O sistema deve dar opção de filtrar os compartilhamentos que foram criados pelo usuário
- O sistema deve dar opção de filtrar os compartilhamentos que o usuário é membro
- O sistema deva dar opção de editar os compartilhamentos que foram criados pelo usuário
- O sistema deve dar opção opção de adicionar membros aos compartilhamentos que foram criados pelo usuário
- O sistema deve exibir ações (editar, adicionar membro) desabilitadas para compartilhamentos do quais não foi criado pelo usuário
- A listagem deve ser em formato de tabela
- A tabela deve conter as seguintes colunas:
  - Nome do compartilhamento
  - Data de criação
  - Número de membros / número máximo de membros
  - Data de vencimento
  - Valor total
  - Valor por membro
  - Ações

## **Fluxo principal**

1. O caso de uso se inicia quando o usuário clica no botão "Compartilhamentos".
2. O sistema exibe a lista de compartilhamentos do usuário.
3. O caso de uso é encerrado.

## **Fluxo alternativo**

### **Nenhum compartilhamento**

1. O sistema exibe uma mensagem informando que o usuário não possui compartilhamentos.
2. O caso de uso é encerrado.

## **Pós-condições**

- O usuário visualiza a lista de compartilhamentos de streaming.
