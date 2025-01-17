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
  - **architecture/**: Documentos de arquitetura.
  - **guidelines/**: Diretrizes do projeto.
  - **manuals/**: Manuais de uso.
    - **developer/**: Manuais para desenvolvedores.
    - **user/**: Manuais para usuários.
  - **requirements/**: Requisitos do projeto.
    - **diagrams/**: Diagramas do projeto.
    - **functional/**: Requisitos funcionais.
    - **non-functional/**: Requisitos não funcionais.

## Padrão de Nomenclatura
- **Artefatos de Requisitos**:
  - Formato: `REQ_<id>_<nome_do_requisito>.md`
  - Exemplos:
    - `REQ_001_Login.md`
    - `REQ_002_Registro.md`

- **Artefatos de BPMN**:
  - Formato: `BPMN_<id>_<nome_do_fluxo>.md`
  - Exemplos:
    - `BPMN_001_AutenticacaoDeUsuario.md`

## Glossário
- **Pessoa Idoso:** Usuário primário do sistema, com acesso total a todas as funcionalidades de gerenciamento pessoal.
- **Responsável:** Familiar que auxilia o idoso, com permissão para gerenciar eventos e rotinas.
- **Cuidador:** Profissional de saúde com acesso limitado a informações diárias e alertas.
- **Sinais Vitais:** Dados de monitoramento de saúde, como pressão arterial, frequência cardíaca e saturação de oxigênio.
- **Evento:** Atividades agendadas como consultas médicas, exercícios e terapias.
- **Rotina de Hábitos:** Conjunto de atividades diárias configuradas para promover saúde física e mental.
- **Alerta:** Notificação automática gerada pelo sistema para lembrar o usuário de eventos ou situações de risco.
- **Prescrição Médica:** Documento com a indicação de medicamentos e dosagens recomendadas pelo médico do idoso, anexado ao perfil do usuário para controle de saúde.
