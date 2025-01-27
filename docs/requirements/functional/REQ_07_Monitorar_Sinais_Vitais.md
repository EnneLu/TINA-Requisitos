### Especificação de Caso de Uso: Monitorar Sinais Vitais  

**1. Descrição do Caso de Uso**  
**COMO** Pessoa Idosa Independente/Responsável/Cuidador  
**QUERO** Monitorar os sinais vitais durante a realização da rotina de hábitos  
**PARA** Acompanhar minha saúde e receber alertas automáticos caso os valores estejam fora dos parâmetros normais.  

**2. Pré-condições**  
- O usuário deve estar cadastrado e autenticado no sistema.  
- O dispositivo de monitoramento deve estar devidamente configurado e conectado ao sistema.  

**3. Fluxo Principal**  
1. O usuário inicia a rotina de hábitos no sistema.  
2. O sistema solicita dados dos sinais vitais ao dispositivo conectado.  
3. O dispositivo fornece as medições ao sistema.  
4. O sistema processa os dados e verifica se estão dentro dos parâmetros normais.  
5. Se os valores estiverem normais, os dados são armazenados no histórico do usuário.  
6. Se os valores estiverem fora dos parâmetros normais, o sistema emite um alerta para o usuário e para os responsáveis cadastrados.  
7. O usuário finaliza a rotina de hábitos.  

**4. Fluxo Alternativo**  
4a. Caso o dispositivo não esteja disponível ou não responda:  
   1. O sistema exibe uma mensagem de erro informando a indisponibilidade do dispositivo.  
   2. O usuário pode optar por tentar novamente ou registrar os sinais vitais manualmente.  

**5. Pós-condições**  
- Os sinais vitais são registrados no sistema.  
- Alertas são enviados, se necessário.  

**6. Regras de Negócio**  
- **RN01** - Os dispositivos de monitoramento devem estar homologados pelo sistema.  
- **RN02** - O sistema deve validar os valores recebidos com base em limites pré-configurados por profissionais de saúde.  
- **RN03** - Alertas devem ser emitidos via notificação sonora e mensagem para os responsáveis em caso de anomalia nos sinais vitais.  
- **RN04** - O usuário deve poder visualizar um histórico consolidado de suas medições anteriores.  

**7. Requisitos Não Funcionais**  
- O monitoramento deve ocorrer em tempo real com uma latência máxima de 5 segundos para a obtenção de dados.  
- O sistema deve garantir a segurança e confidencialidade dos dados transmitidos e armazenados, seguindo padrões como a LGPD.  

---

### Definições de privacidade  

**Identificação dos dados pessoais e sensíveis**  
- Exibe algum dado pessoal? Quais?  
  - Nome do usuário (associado ao registro), data e hora das medições.  
- Exibe algum dado pessoal sensível? Quais?  
  - Sinais vitais, como frequência cardíaca, pressão arterial, saturação de oxigênio e outros dados de saúde.  

**Consentimento do usuário e a permissão de acesso**  
- Tem consentimento?  
  - Sim, o consentimento é obtido no momento do cadastro e aceitação do uso do dispositivo para monitoramento de sinais vitais.  
- Forma de acesso?  
  - Apenas o usuário autenticado e os responsáveis autorizados têm acesso aos dados.  

**Segurança dos dados dentro do processo de tratamento de dados**  
- **Coleta**:  
  - Como será feito?  
    - Os dados serão coletados por dispositivos homologados e transmitidos para o sistema via conexão segura (e.g., Bluetooth com autenticação ou APIs protegidas).  
- **Armazenamento**:  
  - Como será feito?  
    - Os dados serão armazenados em um banco de dados seguro, com criptografia aplicada a informações sensíveis (e.g., AES-256).  
- **Processamento**:  
  - Como será feito?  
    - Os dados serão processados em servidores seguros para análise em tempo real. Todas as operações serão registradas em logs de auditoria.  
- **Compartilhamento**:  
  - **Interno**:  
    - Os dados podem ser acessados pelo sistema para emissão de alertas e visualização no histórico do usuário.  
  - **Externo**:  
    - Os dados não serão compartilhados com terceiros sem o consentimento explícito do usuário.  
  - **Internacional**:  
    - Não haverá transferência internacional de dados.  
- **Eliminação dos dados**:  
  - Os dados serão eliminados a pedido do usuário ou após o período definido nas políticas do sistema, garantindo a exclusão segura e completa do banco de dados.  
