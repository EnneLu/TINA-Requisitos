### Especificação de Caso de Uso: Gerenciar Medicamento

**1. Descrição do Caso de Uso**  
**COMO** Pessoa Idosa Independente ou Responsável  
**QUERO** Registrar, atualizar ou excluir os medicamentos da pessoa idosa  
**PARA** Organizar e garantir o acompanhamento correto da medicação diária.  

**2. Pré-condições**  
- O usuário deve estar autenticado no sistema.  
- Deve haver pelo menos uma pessoa idosa vinculada ao perfil do usuário.  

**3. Fluxo Principal**  
1. O usuário acessa a funcionalidade de gerenciamento de medicamentos no perfil da pessoa idosa.  
2. O sistema exibe a lista de medicamentos já cadastrados (caso existam).  
3. O usuário realiza uma das seguintes ações:  
   - **Adicionar Medicamento**:  
     1. O usuário informa os dados do medicamento, como:  
        - Nome do medicamento.  
        - Quantidade necessária (ex.: 1 comprimido, 10 mL).  
        - Dias da semana em que o medicamento deve ser administrado.  
     2. O sistema valida os dados inseridos.  
     3. O sistema salva o medicamento nos dados da pessoa idosa.  
   - **Atualizar Medicamento**:  
     1. O usuário seleciona um medicamento da lista.  
     2. O usuário edita os dados do medicamento (nome, quantidade ou dias da semana).  
     3. O sistema salva as alterações realizadas.  
   - **Excluir Medicamento**:  
     1. O usuário seleciona um medicamento da lista.  
     2. O sistema solicita confirmação da exclusão.  
     3. O usuário confirma, e o medicamento é removido dos dados da pessoa idosa.  

**4. Fluxo Alternativo**  
3a. Caso algum dado obrigatório não seja preenchido ou seja inválido:  
   1. O sistema exibe uma mensagem de erro indicando os campos a serem corrigidos.  

**5. Pós-condições**  
- Os medicamentos cadastrados são exibidos na rotina diária da pessoa idosa.  
- As informações sobre os medicamentos ficam salvas e atualizadas no sistema.  

**6. Regras de Negócio**  
- **RN01** - Cada medicamento deve estar associado a pelo menos um dia da semana.  
- **RN02** - O sistema deve permitir registrar múltiplos medicamentos para a mesma pessoa idosa.  
- **RN03** - Somente usuários responsáveis podem gerenciar medicamentos vinculados às pessoas idosas.  

**7. Requisitos Não Funcionais**  
- O sistema deve exibir atualizações em até 3 segundos após qualquer ação.  
- A funcionalidade deve ser responsiva e funcionar adequadamente em dispositivos móveis e desktop.  
- As alterações realizadas devem ser registradas para fins de auditoria.  

**8. Diagramas**  
- [Estado](https://github.com/EnneLu/TINA-Requisitos/blob/main/docs/requirements/diagrams/Estado/img/ES_02_Remedio.png)
