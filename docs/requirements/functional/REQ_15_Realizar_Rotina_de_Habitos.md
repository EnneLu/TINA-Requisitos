### Especificação de Caso de Uso: Realizar Rotina de Hábitos

**1. Descrição do Caso de Uso**  
**COMO** Pessoa Idosa Independente/Responsável/Cuidador  
**QUERO** Executar os hábitos planejados para o dia  
**PARA** Seguir minha rotina de forma organizada e monitorar minha saúde durante a execução.  

**2. Pré-condições**  
- O usuário deve estar autenticado no sistema.  
- Devem existir hábitos previamente cadastrados no sistema e agendados para o dia.  
- O dispositivo de monitoramento de sinais vitais deve estar configurado e conectado (se aplicável).  

**3. Fluxo Principal**  
1. O usuário acessa a funcionalidade de rotina de hábitos.  
2. O sistema exibe a lista de hábitos planejados para o dia.  
3. O usuário seleciona um hábito para iniciar.  
4. O sistema inicia a execução do hábito, monitorando os sinais vitais (se aplicável).  
5. O sistema verifica os sinais vitais em tempo real:  
   - Se os valores estiverem dentro dos parâmetros normais, o sistema registra o progresso.  
   - Se os valores estiverem fora dos parâmetros normais, o sistema emite um alerta ao usuário e aos responsáveis.  
6. O usuário conclui a execução do hábito.  
7. O sistema atualiza o status do hábito como "Concluído".  

**4. Fluxo Alternativo**  
4a. Caso o dispositivo de monitoramento de sinais vitais não esteja disponível ou conectado:  
   1. O sistema exibe uma mensagem informando a indisponibilidade do monitoramento.  
   2. O usuário pode optar por continuar a execução sem o monitoramento.  

5a. Caso um alerta seja emitido:  
   1. O sistema registra o evento no histórico do usuário.  
   2. O sistema notifica os responsáveis por meio do canal configurado (e-mail, SMS, ou notificação no aplicativo).  

**5. Pós-condições**  
- O hábito é registrado como concluído no sistema.  
- Os sinais vitais (se monitorados) são armazenados no histórico do usuário.  
- Alertas são enviados, se necessário.  

**6. Regras de Negócio**  
- **RN01** - Apenas hábitos planejados para o dia podem ser iniciados.  
- **RN02**  Alertas devem ser emitidos para os responsáveis caso os sinais vitais estejam fora dos parâmetros normais.  
- **RN03** - A execução de hábitos deve ser registrada no histórico do usuário.  

**7. Requisitos Não Funcionais**  
- O monitoramento de sinais vitais deve ocorrer em tempo real, com uma latência máxima de 5 segundos.  
- O sistema deve ser responsivo e acessível em diferentes dispositivos.  
- Alertas devem ser enviados imediatamente, com tempo máximo de 2 segundos após a detecção de valores fora do padrão.  
