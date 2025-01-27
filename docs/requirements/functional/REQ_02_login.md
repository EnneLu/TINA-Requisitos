### Especificação de Caso de Uso: Login

**1. Descrição do Caso de Uso**  
**COMO** Usuário  
**QUERO** Realizar login no sistema  
**PARA** Acessar minhas informações de forma segura.  

**2. Pré-condições**  
- O usuário deve estar cadastrado no sistema.  

**3. Fluxo Principal**  
1. O usuário acessa a tela de login.  
2. O usuário insere e-mail e senha.  
3. O sistema valida as credenciais.  
4. O sistema concede acesso ao usuário.  

**4. Fluxo Alternativo**  
3a. Se as credenciais forem inválidas:  
  3a.1. O sistema exibe uma mensagem de erro.  
  3a.2. Após múltiplas tentativas falhas, o sistema bloqueia temporariamente a conta.  

**5. Pós-condições**  
- O usuário é autenticado com sucesso.  

**6. Regras de Negócio**  
- **RN01** - A senha deve ser armazenada de forma criptografada.  
- **RN02** - Após 5 tentativas falhas, a conta deve ser bloqueada por segurança.

**7. Requisitos Não Funcionais**  
- O sistema deve ser responsivo e acessível em diferentes dispositivos, incluindo smartphones e tablets.  