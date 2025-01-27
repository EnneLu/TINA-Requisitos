### Especificação de Caso de Uso: Visualizar Rotina Diária  

**1. Descrição do Caso de Uso**  
**COMO** Pessoa Idosa Independente/Responsável/Cuidador  
**QUERO** Visualizar e filtrar informações sobre minha rotina diária  
**PARA** Acompanhar atividades realizadas, medicamentos tomados e eventos planejados.  

**2. Pré-condições**  
- O usuário deve estar cadastrado e autenticado no sistema.  

**3. Fluxo Principal**  
1. O usuário acessa a Área do Idoso.  
2. O sistema exibe as informações diárias, incluindo atividades, medicamentos e eventos.  
3. O usuário seleciona filtros para visualizar informações específicas.  
4. O sistema exibe os resultados conforme os filtros aplicados.  
5. O usuário pode selecionar uma atividade específica para mais detalhes.  

**4. Fluxo Alternativo**  
4a. Caso não haja registros disponíveis:  
  4a.1. O sistema exibe uma mensagem informando a ausência de dados registrados.  
  4a.2. O usuário pode cadastrar uma nova atividade.  

**5. Pós-condições**  
- As informações filtradas são exibidas conforme a necessidade do usuário.  
- O usuário tem acesso ao histórico completo de suas atividades.  

**6. Regras de Negócio**  
- **RN01** - O sistema deve permitir a filtragem por data, tipo de atividade e status (concluído/não concluído).  
- **RN02** - Apenas usuários autorizados podem visualizar determinadas informações sensíveis.  
- **RN03** - Os dados registrados devem estar organizados de forma cronológica.  

**7. Requisitos Não Funcionais**  
- O sistema deve garantir a privacidade e segurança das informações do usuário, conforme a LGPD.  
- A interface deve ser responsiva para diferentes dispositivos.  

---

### Definições de privacidade  

**Identificação dos dados pessoais e sensíveis**  
- Exibe algum dado pessoal? Quais?  
  - Nome do usuário associado à rotina, datas e horários das atividades, medicamentos tomados e eventos planejados.  
- Exibe algum dado pessoal sensível? Quais?  
  - Informações sobre medicamentos tomados, atividades de saúde e eventos médicos relacionados à saúde.  

**Consentimento do usuário e a permissão de acesso**  
- Tem consentimento?  
  - Sim, o consentimento é obtido no momento do cadastro e inclui a visualização e tratamento de dados relacionados à rotina diária.  
- Forma de acesso?  
  - Apenas usuários autenticados têm acesso às informações, e os dados sensíveis só podem ser visualizados por pessoas autorizadas (ex.: Responsáveis/Cuidadores).  

**Segurança dos dados dentro do processo de tratamento de dados**  
- **Coleta**:  
  - Como será feito?  
    - Os dados são registrados previamente pelo usuário, por cuidadores ou importados de dispositivos conectados ao sistema.  
- **Armazenamento**:  
  - Como será feito?  
    - Os dados são armazenados em banco de dados seguro com criptografia aplicada a informações sensíveis, garantindo a integridade e confidencialidade.  
- **Processamento**:  
  - Como será feito?  
    - O sistema processará os filtros em tempo real e garantirá que os dados exibidos respeitem as permissões e configurações de privacidade do usuário.  
- **Compartilhamento**:  
  - **Interno**:  
    - Os dados podem ser acessados pelo usuário e pelos responsáveis autorizados para consulta e acompanhamento.  
  - **Externo**:  
    - Não haverá compartilhamento de dados com terceiros sem o consentimento explícito do usuário.  
  - **Internacional**:  
    - Não haverá transferência internacional de dados.  
- **Eliminação dos dados**:  
  - Os dados podem ser excluídos a pedido do usuário ou automaticamente conforme o prazo definido nas políticas do sistema, utilizando métodos seguros de descarte.  
