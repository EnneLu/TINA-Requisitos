### Especificação de Caso de Uso: Emitir Alerta

**1. Descrição do Caso de Uso**  
**COMO** Pessoa Idosa Independente/Responsável/Cuidador  
**QUERO** Receber alertas em tempo real sobre alterações nos batimentos cardíacos durante a execução de hábitos  
**PARA** Garantir a segurança e saúde da pessoa idosa ao identificar anomalias rapidamente.  

**2. Pré-condições**  
- O usuário deve estar autenticado no sistema.  
- O dispositivo de monitoramento de sinais vitais deve estar configurado e conectado ao sistema.  
- O hábito monitorado deve estar em execução.  

**3. Fluxo Principal**  
1. O usuário inicia a execução de um hábito.  
2. O sistema monitora os batimentos cardíacos em tempo real.  
3. O sistema compara os valores monitorados com os limites definidos por profissionais de saúde:  
   - Se os valores estiverem fora do intervalo considerado normal, o sistema emite um alerta.  
4. O alerta é exibido para o usuário e registrado como uma notificação.  
5. O sistema notifica os responsáveis cadastrados (se configurado).  

**4. Fluxo Alternativo**  
3a. Caso o dispositivo de monitoramento não esteja conectado:  
   1. O sistema exibe uma mensagem informando a indisponibilidade do monitoramento.  
   2. O hábito pode ser executado sem monitoramento, sem emissão de alertas.  

**5. Pós-condições**  
- O alerta é registrado no histórico de notificações do sistema.  
- Os responsáveis recebem as notificações caso habilitados.  

**6. Regras de Negócio**  
- **RN01** - O sistema deve validar os batimentos monitorados com base em limites personalizados definidos por profissionais de saúde.  
- **RN02** - Alertas devem ser enviados aos responsáveis por meio dos canais configurados (e-mail, SMS, ou notificação no aplicativo).  
- **RN03** - Todas as notificações de alerta devem ser armazenadas para consulta posterior.  

**7. Requisitos Não Funcionais**  
- A emissão de alertas deve ocorrer em até 2 segundos após a detecção de valores fora do padrão.  
- O sistema deve garantir alta disponibilidade para o monitoramento em tempo real (99,9%).  
- A interface de notificações deve ser responsiva e acessível em diferentes dispositivos, incluindo smartphones e tablets.  
