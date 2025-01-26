### Especificação de Caso de Uso: Cadastrar Usuário

**1. Descrição do Caso de Uso**  
**COMO** Pessoa Idosa Independente/Responsável/Cuidador  
**QUERO** Me cadastrar no sistema  
**PARA** Acessar e utilizar as funcionalidades disponíveis de acordo com meu perfil.  

**2. Pré-condições**  
- O usuário deve acessar a página de cadastro.  

**3. Fluxo Principal**  
1. O sistema solicita que o usuário selecione seu perfil entre as opções: Pessoa Idosa Independente, Responsável ou Cuidador.
2. O sistema exibe o formulário de cadastro de acordo com o perfil selecionado, com os seguintes campos obrigatórios para preenchimento:
   - Nome completo
   - Data de nascimento
   - E-mail
   - Telefone
   - Senha
   - Confirmar senha
3. O usuário preenche os campos obrigatórios com as informações necessárias.  
4. O sistema valida os dados inseridos, incluindo:
   - Verificação de e-mail único no sistema.
   - Verificação de correspondência entre as senhas.
   - Formatação válida para e-mail e telefone.
   - Política de segurança para a senha (mínimo de caracteres, complexidade, etc.).
5. O sistema confirma o cadastro e envia uma notificação de sucesso, direcionando o usuário para a tela de login.

**4. Fluxo Alternativo**  
4a. Se os dados estiverem incorretos ou incompletos:
   1. O sistema exibe mensagens de erro indicando quais campos precisam ser corrigidos.
   2. O sistema não prossegue com o cadastro até que todos os campos obrigatórios sejam preenchidos corretamente.

4b. Se o e-mail já estiver registrado no sistema:
   1. O sistema exibe uma mensagem informando que o e-mail já está em uso e solicita que o usuário insira um e-mail diferente.

4c. Se as senhas não corresponderem:
   1. O sistema exibe uma mensagem de erro indicando que as senhas não são iguais e solicita que o usuário corrija.

**5. Pós-condições**  
- O usuário está cadastrado no sistema e pode realizar login.  
- As informações do usuário são armazenadas no banco de dados do sistema.

**6. Regras de Negócio**  
- **RN01** - O e-mail deve ser único no sistema.  
- **RN02** -  A senha deve atender às políticas de segurança definidas pelo sistema, incluindo a combinação de letras, números e caracteres especiais, com um mínimo de 8 caracteres.
- **RN03** - A confirmação da senha deve ser idêntica à senha inserida no campo anterior.
- **RN04** - O telefone deve ser validado conforme o formato padrão do país ou região do usuário.

**7. Requisitos Não Funcionais**  
- O tempo de resposta para validar e confirmar o cadastro não deve exceder 3 segundos.
- O sistema deve ser responsivo e acessível em diferentes dispositivos, incluindo smartphones e tablets.  
- O sistema deve garantir a segurança e confidencialidade dos dados pessoais dos usuários, em conformidade com a LGPD.