## Contexto
O projeto consiste na análise e desenvolvimento do TINA, um aplicativo projetado para apoiar a saúde de pessoas idosas. O principal objetivo do sistema é proporcionar um ambiente de bem-estar, promovendo uma rotina saudável e auxiliando tanto os usuários quanto os cuidadores por meio de funcionalidades específicas para a saúde física e mental.

## Problema
A gestão manual das rotinas de saúde e bem-estar dos idosos apresenta diversos desafios, como:

- Falta de acompanhamento eficaz das atividades diárias.
- Dificuldade em manter uma rotina saudável e organizada.
- Esquecimento de consultas e medicações.
- Ausência de um sistema de monitoramento em situações de emergência.

Esses problemas afetam a autonomia dos idosos e a capacidade de cuidadores e familiares de monitorar e apoiar de forma eficiente.

## Estrutura de Pastas

- **docs/**: Documentação do projeto.
  - **diagrams/**: Diagramas de requisitos.
    - **Estado/**: Diagramas de estado.
    - **NFR/**: Diagramas NFR.
    - **UC/**: Diagramas de casos de uso.
  - **functional/**: Requisitos funcionais.
  - **non_functional/**: Requisitos não funcionais.

## Padrão de Nomenclatura
- **Artefatos de Requisitos**:
  - Formato: `REQ_<id>_<nome_do_requisito>.md`
  - Exemplos:
    - `REQ_01_Login.md`
    - `REQ_02_Registro.md`

- **Artefatos de BPMN**:
  - Formato: `BPMN_<id>_<nome_do_fluxo>.md`
  - Exemplos:
    - `BPMN_01_AutenticacaoDeUsuario.md`

- **Artefatos de Estado**:
  - Formato: `ES_<id>_<nome_do_fluxo>.md`
  - Exemplos:
    - `ES_01_AutenticacaoDeUsuario.md`

## Glossário
- **Pessoa Idosa:** Usuário primário do sistema, com acesso total a todas as funcionalidades de gerenciamento pessoal.
- **Responsável:** Familiar que auxilia o idoso, com permissão para gerenciar eventos e rotinas.
- **Cuidador:** Profissional de saúde com acesso limitado a informações diárias e alertas.
- **Sinais Vitais:** Dados de monitoramento de saúde, como pressão arterial, frequência cardíaca e saturação de oxigênio.
- **Evento:** Atividades agendadas como consultas médicas, exercícios e terapias.
- **Hábitos**: Conjunto de atividades diárias configuradas para promover saúde física e mental.
- **Rotina Diária:**: Eventos, medicamento e hábitos planejados para o dia.
- **Alerta:** Notificação automática gerada pelo sistema para lembrar o usuário de eventos ou situações de risco.
- **Prescrição Médica:** Documento com a indicação de medicamentos e dosagens recomendadas pelo médico do idoso, anexado ao perfil do usuário para controle de saúde.
