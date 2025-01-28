### Especificação de Caso de Uso: Gerenciar Evento  

**1. Descrição do Caso de Uso**  
**COMO** Pessoa Idosa Independente/Responsável/Cuidador  
**QUERO** Cadastrar eventos no sistema  
**PARA** Organizar minha rotina de saúde.  

**2. Pré-condições**  
- O usuário deve estar autenticado.  

**3. Fluxo Principal**  
1. O usuário acessa a funcionalidade de cadastro de tarefas.  
2. O sistema exibe uma lista de tipos de tarefas que podem ser criadas (como hábito, evento ou medicamento).  
3. O usuário seleciona a opção de evento.  
4. O sistema solicita os seguintes dados:  
   - Descrição do evento (ex.: consulta com endocrinologista)  
   - Data específica do evento  
   - Horário específico do evento  
   - Local onde o evento ocorrerá (opcional)  
   - Status do evento (Em aberto, Concluído e Cancelado)  
5. O usuário preenche os campos obrigatórios e confirma a criação do evento.  
6. O sistema valida os dados inseridos e confirma que todas as informações estão corretas.  
7. O sistema salva o evento no calendário do usuário e envia uma notificação de confirmação.  

**4. Fluxo Alternativo**  
4a. Caso algum campo obrigatório não seja preenchido:  
   1. O sistema exibe uma mensagem de erro.  

4b. Caso o usuário opte por excluir um evento:  
   1. O sistema solicita confirmação antes de excluir permanentemente o evento.  
   2. O usuário confirma a exclusão e o hábito é removido da lista de eventos.  
   3. O sistema envia uma notificação de confirmação da exclusão.  

**5. Pós-condições**  
- O evento é salvo corretamente no sistema e pode ser editado ou excluído posteriormente.  

**6. Regras de Negócio**  
- **RN01** - Todos os campos obrigatórios devem ser preenchidos antes de salvar o evento.  
- **RN02** - O sistema deve permitir que o evento seja editado ou excluído após sua criação.  
- **RN03** - O campo Status deve permitir as opções "aberto", "concluído" e "cancelado".  
- **RN04** - O sistema deve garantir que o evento não possa ser salvo sem todos os dados obrigatórios preenchidos corretamente.  

**7. Requisitos Não Funcionais**  
- O sistema deve ser responsivo e acessível em diferentes dispositivos, incluindo smartphones e tablets.  
- O sistema deve garantir a confidencialidade e integridade das informações dos eventos, conforme as leis de proteção de dados (LGPD).  

**8. Diagramas**  
- [Estado](https://github.com/EnneLu/TINA-Requisitos/blob/main/docs/requirements/diagrams/Estado/img/ES_03_Evento.png)

---

### Definições de privacidade  

**Identificação dos dados pessoais e sensíveis**  
- Exibe algum dado pessoal? Quais?  
  - Descrição do evento, data, horário e local.  
- Exibe algum dado pessoal sensível? Quais?  
  - Nenhum dado sensível identificado neste caso de uso.  

**Consentimento do usuário e a permissão de acesso**  
- Tem consentimento?  
  - Sim, o consentimento é obtido no momento do cadastro do usuário, permitindo o armazenamento e tratamento de dados de eventos pessoais.  
- Forma de acesso?  
  - Apenas o usuário autenticado pode acessar, criar, editar ou excluir seus próprios eventos.  

**Segurança dos dados dentro do processo de tratamento de dados**  
- **Coleta**:  
  - Como será feito?  
    - Por meio de formulários preenchidos pelo usuário autenticado, utilizando conexão segura (HTTPS).  
- **Armazenamento**:  
  - Como será feito?  
    - Os dados de eventos serão armazenados em um banco de dados seguro com criptografia aplicada aos dados sensíveis.  
- **Processamento**:  
  - Como será feito?  
    - As operações de criação, edição e exclusão de eventos serão realizadas em servidores seguros com registro de logs para auditoria.  
- **Compartilhamento**:  
  - **Interno**:  
    - Os eventos criados são visíveis apenas ao usuário autenticado e a serviços do sistema relacionados à notificação ou organização de dados.  
  - **Externo**:  
    - Não haverá compartilhamento de dados com terceiros sem consentimento explícito do usuário.  
  - **Internacional**:  
    - Não haverá transferência internacional de dados.  
- **Eliminação dos dados**:  
  - Os dados dos eventos podem ser excluídos diretamente pelo usuário ou automaticamente após o prazo definido no sistema. A exclusão será feita de forma segura, garantindo a remoção completa do banco de dados.  
