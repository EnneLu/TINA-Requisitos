### Especificação de Caso de Uso: Visualizar Rotina

**1. Descrição do Caso de Uso**  
**COMO** Pessoa Idosa Independente/Responsável/Cuidador  
**QUERO** Visualizar e filtrar informações sobre minha rotina diária
**PARA** Acompanhar atividades realizadas, medicamentos tomados e eventos planejados.

**2. Pré-condições**  
- O usuário deve estar cadastrado e autenticado no sistema.

**3. Fluxo Principal**  
1. O usuário acessa a funcionalidade de rotina no sistema. 
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
