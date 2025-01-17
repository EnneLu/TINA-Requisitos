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
    - **design/**: Documentos de design.
    - **functional/**: Requisitos funcionais.
    - **non-functional/**: Requisitos não funcionais.

- **scripts/**: Scripts do projeto.
  - **build/**: Scripts de build.
  - **migration/**: Scripts de migração.
  - **seed/**: Scripts de seed.

- **src/**: Código-fonte do projeto.
  - **application/**: Lógica de aplicação.
    - **use-cases/**: Casos de uso.
    - **dto/**: Data Transfer Objects.
    - **interfaces/**: Interfaces que os casos de uso dependem.
  - **domain/**: Lógica de domínio.
    - **entities/**: Entidades do domínio.
    - **enums/**: Enums do domínio.
    - **models/**: Modelos do domínio.
    - **value-objects/**: Objetos de valor do domínio.
  - **infra/**: Infraestrutura.
    - **configs/**: Configurações.
    - **databases/**: Bancos de dados.
    - **repositories/**: Repositórios.
    - **services/**: Serviços de infraestrutura.
  - **presentation/**: Camada de apresentação.
    - **controllers/**: Controladores.
    - **middlewares/**: Middlewares.
    - **ui/**: Interface do usuário.

- **tests/**: Testes do projeto.
  - **e2e/**: Testes end-to-end.
  - **integration/**: Testes de integração.
  - **unit/**: Testes unitários.


## Padrão de Nomenclatura
- **Artefatos de Requisitos**:
  - Formato: `REQ_<id>_<nome_do_requisito>.md`
  - Exemplos:
    - `REQ_001_Login.md`
    - `REQ_002_Registro.md`

## Commits

Os commits devem seguir o padrão [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/):

- **feat**: Para novas funcionalidades.
  - Exemplo: `feat: adicionar funcionalidade de monitoramento de sinais vitais`
- **fix**: Para correção de bugs.
  - Exemplo: `fix: corrigir erro de autenticação na API`
- **chore**: Para tarefas de manutenção ou organização.
  - Exemplo: `chore: reorganizar estrutura de pastas`
- **docs**: Para atualizações na documentação.
  - Exemplo: `docs: adicionar definição de requisitos no README`
- **test**: Para adição ou modificação de testes.
  - Exemplo: `test: adicionar testes para a funcionalidade de login`

## Branches

Use o padrão: `<tipo>/<descrição-curta>`

- **Tipos**:
  - **feature**: Para desenvolvimento de novas funcionalidades.
  - **fix**: Para correção de bugs.
  - **hotfix**: Para correções rápidas em produção.
  - **release**: Para preparar uma versão para produção.

- **Exemplos**:
  - `feature/cadastro-usuario`
  - `fix/corrigir-autenticacao`
  - `hotfix/corrigir-bug-emergencial`

## Glossário