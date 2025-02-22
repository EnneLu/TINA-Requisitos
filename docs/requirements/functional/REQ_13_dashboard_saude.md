### Especificação de Caso de Uso: Dashboard de Saúde  

**1. Descrição do Caso de Uso**  
**COMO** Pessoa Idosa Independente/Responsável/Cuidador  
**QUERO** Visualizar um Dashboard de Saúde  
**PARA** Monitorar minhas métricas de saúde e hábitos de forma visual e interativa.  

**2. Pré-condições**  
- O usuário deve estar cadastrado e autenticado no sistema.  
- O sistema deve ter dados de sinais vitais e hábitos registrados.  

**3. Fluxo Principal**  
1. O usuário acessa a funcionalidade do Dashboard de Saúde.  
2. O sistema exibe o Dashboard de Saúde, contendo gráficos e métricas relevantes.  
3. O painel exibe dados de sinais vitais como:  
   - Pressão arterial  
   - Frequência cardíaca  
   - Saturação de oxigênio  
   - Temperatura corporal  
4. O painel exibe gráficos com as tendências desses sinais vitais ao longo do tempo, com diferentes intervalos (diário, semanal, mensal).  
5. O painel também exibe gráficos relacionados aos hábitos do usuário, como:  
   - Frequência de medicação  
   - Atividades físicas realizadas  
   - Alimentação  
   - Sono  
6. O usuário pode interagir com os gráficos para filtrar e visualizar métricas específicas ou um período de tempo diferente.  
7. O sistema atualiza os gráficos de forma dinâmica sempre que novos dados são registrados.  

**4. Fluxo Alternativo**  
4a. Caso não haja dados registrados para algum sinal vital ou hábito:  
   1. O sistema exibe uma mensagem informando que não há dados suficientes para exibir gráficos ou tendências.  

4b. Caso o usuário deseje comparar dados de diferentes períodos:  
   1. O sistema permite ao usuário selecionar diferentes intervalos de tempo (ex.: comparar uma semana com o mês anterior) para visualizar as mudanças nas métricas.  

**5. Pós-condições**  
- O usuário visualiza o Dashboard de Saúde atualizado com seus dados e tendências.  
- O sistema armazena as interações do usuário, caso o usuário escolha visualizar gráficos de períodos ou métricas específicas.  

**6. Regras de Negócio**  
- **RN01** - O sistema deve garantir que os gráficos sejam atualizados em tempo real sempre que novos dados forem registrados.  
- **RN02** - O sistema deve permitir a personalização de filtros para análise de dados, incluindo intervalos de tempo e categorias de sinais vitais/hábitos.  
- **RN03** - O sistema deve garantir que os dados do painel estejam sempre atualizados e correspondam aos dados mais recentes registrados.  

**7. Requisitos Não Funcionais**  
- O sistema deve ser capaz de exibir gráficos de maneira rápida, com tempos de resposta não superiores a 2 segundos para cada atualização de gráfico.  
- O Dashboard deve ser responsivo e acessível em diferentes dispositivos, incluindo smartphones, tablets e desktops.  
- O sistema deve garantir que os dados apresentados no Dashboard de Saúde estejam de acordo com as regulamentações de privacidade e segurança de dados, como a LGPD.  

---

### Definições de privacidade  

**Identificação dos dados pessoais e sensíveis**  
- Exibe algum dado pessoal? Quais?  
  - Nome do usuário associado às métricas, intervalos de tempo e categorias de hábitos.  
- Exibe algum dado pessoal sensível? Quais?  
  - Sinais vitais (pressão arterial, frequência cardíaca, saturação de oxigênio, temperatura corporal), hábitos de saúde (medicação, atividades físicas, alimentação e sono).  

**Consentimento do usuário e a permissão de acesso**  
- Tem consentimento?  
  - Sim, o consentimento explícito é obtido no momento do cadastro para permitir o monitoramento e exibição dos dados no Dashboard.  
- Forma de acesso?  
  - Apenas usuários autenticados podem acessar o Dashboard de Saúde, e os dados sensíveis são acessíveis apenas pelo titular ou responsáveis autorizados.  

**Segurança dos dados dentro do processo de tratamento de dados**  
- **Coleta**:  
  - Como será feito?  
    - Os dados serão coletados de dispositivos conectados, registros manuais do usuário ou integrações com sistemas parceiros (como dispositivos de monitoramento de saúde).  
- **Armazenamento**:  
  - Como será feito?  
    - Os dados serão armazenados em banco de dados seguro com criptografia aplicada a informações sensíveis (e.g., AES-256).  
- **Processamento**:  
  - Como será feito?  
    - O sistema processará os dados em tempo real para gerar gráficos e métricas, garantindo a consistência e atualização automática. Logs de auditoria serão mantidos.  
- **Compartilhamento**:  
  - **Interno**:  
    - Os dados são acessíveis para visualização e análise apenas pelo usuário e por serviços do sistema necessários para gerar o Dashboard.  
  - **Externo**:  
    - Não haverá compartilhamento com terceiros sem consentimento explícito do usuário.  
  - **Internacional**:  
    - Não haverá transferência internacional de dados.  
- **Eliminação dos dados**:  
  - Os dados podem ser excluídos pelo usuário ou conforme políticas de retenção estabelecidas, garantindo descarte seguro e completo.  
