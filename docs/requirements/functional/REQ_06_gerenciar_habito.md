### Especificação de Caso de Uso: Gerenciar Hábito

**1. Descrição do Caso de Uso**  
**COMO** Pessoa Idosa Independente/Responsável/Cuidador  
**QUERO** Gerenciar meus hábitos de saúde e bem-estar (como alimentação, medicação, exercícios)  
**PARA** Estabelecer uma rotina, garantir que os hábitos sejam realizados com regularidade e receber lembretes conforme configurado.

**2. Pré-condições**  
- O usuário deve estar cadastrado e autenticado no sistema.

**3. Fluxo Principal**  
1. O usuário acessa a funcionalidade de cadastro de tarefas.  
2. O sistema exibe uma lista de tipos de tarefas que podem ser criadas (como hábito, evento ou medicamento).
3. O usuário escolhe adicionar um novo hábito.  
4. O sistema solicita os seguintes dados:  
   - Descrição do hábito (ex.: tomar medicamento, realizar exercício, etc.)  
   - Frequência (diária, semanal, mensal)  
   - Se deve repetir todos os dias (opcional)
   - Horário específico do hábito (opcional)  
   - Dias da semana em que o hábito deve ocorrer (opcional)  
5. O usuário insere as informações e confirma o cadastro do hábito.  
6. O sistema salva as informações do hábito e exibe um resumo dos dados inseridos.  
7. O sistema configura a notificação de lembrete conforme os parâmetros definidos (frequência, horário e dias da semana).  
8. O sistema envia lembretes de acordo com a frequência e horário configurados.

**4. Fluxo Alternativo**  
4a. Caso o usuário não defina uma frequência ou horário:  
   1. O sistema exibe uma mensagem sugerindo a escolha de uma frequência ou horário para garantir o funcionamento da rotina.  
   2. O usuário pode optar por continuar sem essas informações, caso não se aplique. 
 
4b. Caso o usuário opte por excluir um hábito:  
   1. O sistema solicita confirmação antes de excluir permanentemente o hábito.  
   2. O usuário confirma a exclusão e o hábito é removido da lista de hábitos.  
   3. O sistema envia uma notificação de confirmação da exclusão.

**5. Pós-condições**  
- O hábito foi registrado com sucesso no sistema e está disponível na lista de hábitos.  
- O sistema configura e envia lembretes conforme as configurações do usuário.  
- O usuário pode visualizar, editar ou excluir os hábitos conforme necessário.

**6. Regras de Negócio**  
- **RN01** - O sistema deve permitir que o usuário defina a frequência do hábito como diária, semanal ou mensal.  
- **RN02** - O sistema deve permitir que o usuário selecione os dias da semana nos quais o hábito deve ocorrer.  
- **RN03** - O sistema deve permitir a configuração de horários específicos para cada hábito.  
- **RN04** - Os lembretes de hábito devem ser enviados nos dias e horários definidos pelo usuário.  
- **RN05** - O usuário deve ser capaz de editar as informações do hábito ou excluir hábitos a qualquer momento.  
- **RN06** - O sistema deve garantir que um hábito só possa ser excluído após confirmação do usuário.

**7. Requisitos Não Funcionais**  
- O sistema deve ser responsivo e acessível em diferentes dispositivos, incluindo smartphones e tablets.  
- Os lembretes devem ser enviados com pelo menos 10 minutos de antecedência do horário configurado, para garantir tempo suficiente para o usuário se organizar.  
- O sistema deve garantir a segurança e confidencialidade das informações relacionadas aos hábitos do usuário.