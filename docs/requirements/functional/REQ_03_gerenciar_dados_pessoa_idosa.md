### Especificação de Caso de Uso: Gerenciar Dados Pessoa Idosa

**1. Descrição do Caso de Uso**  
**COMO** Pessoa Idosa Independente/Responsável  
**QUERO** Adicionar, atualizar e excluir meus dados pessoais e de saúde  
**PARA** Manter minhas informações sempre atualizadas.

**2. Pré-condições**  
- O usuário deve estar autenticado no sistema.

**3. Fluxo Principal**  
1. O usuário acessa a funcionalidade de gerenciamento de dados.  
2. O sistema exibe as informações atuais do usuário, permitindo a visualização e a edição de dados pessoais e de saúde, como:
   - Nome completo
   - Data de nascimento
   - Endereço
   - Informações de contato (telefone, e-mail)
   - Histórico de condições de saúde
   - Medicamentos em uso
   - Alergias
   - Dados de emergências (contatos, condições críticas)
3. O usuário insere ou edita as informações desejadas.  
4. O sistema valida os dados inseridos, verificando:
   - Formatação de dados (telefone, e-mail, etc.)
   - Consistência das informações de saúde (valores numéricos, dados de histórico médico)
5. O sistema salva as alterações e exibe uma confirmação de sucesso.

**4. Fluxo Alternativo**  
4a. Caso algum campo obrigatório não esteja preenchido ou os dados estejam incorretos:
   1. O sistema exibe uma mensagem de erro informando quais campos precisam ser corrigidos.

4b. Caso o usuário deseje excluir dados:
   1. O sistema solicita confirmação antes de excluir os dados.
   2. O usuário confirma a exclusão, e o sistema remove os dados da base.
   3. O sistema envia uma notificação informando que a exclusão foi realizada com sucesso.

**5. Pós-condições**  
- Os dados do usuário são atualizados no sistema ou removidos conforme solicitado.

**6. Regras de Negócio**  
- **RN01** - Somente usuários autorizados (Pessoa Idosa Independente ou Responsável) podem modificar dados sensíveis.
- **RN02** - As informações devem ser armazenadas de forma segura, com criptografia para dados sensíveis.
- **RN03** - O sistema deve permitir que os dados de saúde sejam atualizados regularmente e que o histórico de alterações seja mantido.

**7. Requisitos Não Funcionais**  
- As operações de gerenciamento de dados devem ser registradas para auditoria.  
- O sistema deve garantir disponibilidade de 99,9% para acesso aos dados.  
- O sistema deve ser responsivo, funcionando corretamente em dispositivos móveis e desktops.
