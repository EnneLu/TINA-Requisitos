### Especificação de Caso de Uso: Confirmar Evento

**1. Descrição do Caso de Uso**  
**COMO** Pessoa Idosa Independente/Responsável/Cuidador  
**QUERO** Confirmar eventos agendados  
**PARA** Garantir que os eventos sejam realizados conforme planejado e que as prescrições médicas estejam anexadas corretamente.

**2. Pré-condições**  
- O usuário deve estar cadastrado e autenticado no sistema.  
- O usuário deve ter uma prescrição médica digitalizada em formato PDF, JPG ou PNG para anexar ao evento.

**3. Fluxo Principal**  
1. O usuário acessa a funcionalidade de confirmação de evento.  
2. O sistema exibe os eventos agendados ou a serem confirmados, com os detalhes necessários para revisão.  
3. O usuário seleciona o evento que deseja confirmar.  
4. O sistema solicita o upload de uma prescrição médica digitalizada (formato PDF, JPG ou PNG), caso não tenha sido anexada anteriormente.  
5. O usuário anexa a prescrição médica (ou confirma que já foi anexada previamente).  
6. O sistema valida o formato e o tamanho do arquivo anexado, garantindo que ele esteja dentro dos requisitos especificados (PDF, JPG ou PNG).  
7. O sistema confirma a obrigatoriedade do anexo e exibe uma mensagem de sucesso após o upload bem-sucedido.  
8. O usuário confirma o evento como concluído ou atualizado, e o sistema registra essa confirmação.

**4. Fluxo Alternativo**  
4a. Caso o usuário não anexe uma prescrição médica, ou anexe em formato incorreto:  
   1. O sistema exibe uma mensagem de erro, informando sobre o tipo de arquivo aceito (PDF, JPG, PNG) e solicita o reenvio do arquivo.  

4b. Caso o arquivo seja muito grande:  
   1. O sistema exibe uma mensagem indicando o limite de tamanho do arquivo e solicita o envio de um arquivo com tamanho adequado.

**5. Pós-condições**  
- O evento é confirmado no sistema e a prescrição médica é anexada corretamente.  
- O sistema valida e registra a prescrição junto ao evento para referência futura.

**6. Regras de Negócio**  
- **RN01** - O sistema deve garantir que apenas arquivos nos formatos PDF, JPG ou PNG sejam aceitos.  
- **RN02** - O sistema deve validar o tamanho do arquivo para garantir que ele não ultrapasse o limite estabelecido (ex.: 5MB).  
- **RN03** - A prescrição médica deve ser anexada ao evento para qualquer alteração ou confirmação relacionada a medicamentos.

**7. Requisitos Não Funcionais**  
- O tempo de resposta para o upload do arquivo não deve exceder 10 segundos.  
- O sistema deve ser capaz de armazenar arquivos de prescrição de forma segura, garantindo a confidencialidade e integridade dos dados, conforme políticas de segurança de dados sensíveis.