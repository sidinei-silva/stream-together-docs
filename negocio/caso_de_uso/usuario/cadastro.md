# Cadastro de Usuário

### **Atores:**

Novo Usuário

### **Entradas:**

Nome, e-mail, senha.

### **Saídas:**

Confirmação de cadastro, mensagem de erro em caso de falha (e-mail já utilizado, senha fraca).

### **Pré-condições:**

Nenhuma

### **Fluxo Principal:**

1. O Novo Usuário seleciona a opção de cadastro na aplicação.
2. O sistema apresenta o formulário de cadastro.
3. O Novo Usuário preenche os detalhes necessários: nome, e-mail e senha.
4. O Novo Usuário submete o formulário.
5. O sistema valida as informações e cria a nova conta.
6. O sistema envia um e-mail de confirmação ao Novo Usuário.
7. O Novo Usuário confirma o e-mail.
8. O sistema confirma a criação da conta e permite o login.

### **Fluxos Alternativos:**

* **E-mail Já Utilizado:** Se o e-mail já estiver em uso, o sistema informa ao usuário para tentar outro e-mail.
* **Dados Inválidos:** Se os dados forem inválidos (ex.: senha muito fraca), o sistema solicita a correção dos dados.