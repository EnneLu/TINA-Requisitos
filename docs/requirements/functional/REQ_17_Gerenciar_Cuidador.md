### Especificação de Caso de Uso: Gerenciar Cuidador

**1. Descrição do Caso de Uso**  
**COMO** Usuário Responsável  
**QUERO** Adicionar, atualizar ou remover cuidadores vinculados à pessoa idosa no qual sou responsável  
**PARA** Gerenciar a equipe de apoio e organizar os dias de acompanhamento do idoso.  

**2. Pré-condições**  
- O responsável deve estar autenticado no sistema.  
- Deve haver pelo menos uma pessoa idosa vinculada ao perfil do responsável.  

**3. Fluxo Principal**  
1. O responsável acessa a funcionalidade de gerenciamento de cuidadores.  
2. O sistema exibe a lista de cuidadores vinculados à pessoa idosa.  
3. O responsável realiza uma das seguintes ações:  
   - **Adicionar Cuidador**:  
     1. O responsável envia um convite ao perfil de cuidador cadastrado no sistema.  
     2. O responsável seleciona os dias da semana em que o cuidador acompanhará o idoso.  
     3. O sistema valida os dados inseridos.  
     4. O sistema vincula o cuidador ao perfil da pessoa idosa.  
   - **Atualizar Cuidador**:  
     1. O responsável seleciona o cuidador da lista.  
     2. O responsável edita os dados ou os dias de acompanhamento.  
     3. O sistema salva as alterações.  
   - **Remover Cuidador**:  
     1. O responsável seleciona o cuidador da lista.  
     2. O sistema solicita confirmação da exclusão.  
     3. O responsável confirma a exclusão, e o cuidador é desvinculado do perfil da pessoa idosa.  

**4. Fluxo Alternativo**  
3a. Caso algum dado obrigatório não seja preenchido ou seja inválido:  
   1. O sistema exibe uma mensagem de erro indicando os campos a serem corrigidos.  

**5. Pós-condições**  
- O cuidador é adicionado, atualizado ou removido no sistema conforme a ação realizada.  
- Os dias de acompanhamento do cuidador estão registrados e atualizados no sistema.  

**6. Regras de Negócio**  
- **RN01** - O responsável só pode gerenciar cuidadores vinculados às pessoas idosas no qual é responsável.  
- **RN02** - Os dias de acompanhamento devem ser especificados para cada cuidador vinculado.  

**7. Requisitos Não Funcionais**  
- O sistema deve exibir as alterações realizadas em até 3 segundos após a ação do usuário.  
- A funcionalidade deve ser responsiva e acessível em dispositivos móveis e desktop.  
- O sistema deve registrar todas as alterações realizadas para fins de auditoria.  
