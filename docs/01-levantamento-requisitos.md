# WantWeb — Sistema de Gerenciamento de Chamados

## 1. Levantamento de Requisitos

### 1.1 Problema

Empresas e equipes que prestam suporte recebem diariamente solicitações de usuários relacionadas a dúvidas, problemas, solicitações e necessidades de atendimento. Quando essas solicitações não são organizadas em um sistema centralizado, pode ocorrer dificuldade para acompanhar os atendimentos, identificar chamados pendentes, controlar prioridades e registrar as soluções realizadas.

O problema identificado é a falta de uma ferramenta simples que permita registrar, organizar, direcionar e acompanhar os chamados desde sua abertura até o encerramento.

O WantWeb será desenvolvido para centralizar o gerenciamento dessas solicitações, permitindo que os usuários registrem chamados e que os atendentes acompanhem uma fila de atendimento, assumam solicitações, registrem interações, atualizem o status e documentem a solução.

O sistema terá como referência conceitos utilizados em ambientes de atendimento e contact center, como organização de filas, distribuição de chamados, prioridade, status e histórico de atendimento, porém com um escopo simplificado e adequado ao projeto acadêmico.

### 1.2 Objetivo do Sistema

O objetivo do WantWeb é desenvolver um sistema web simples para gerenciamento de chamados, permitindo registrar, organizar, acompanhar e encerrar solicitações de atendimento.

O sistema deverá possibilitar que os solicitantes abram chamados e acompanhem seu andamento, enquanto os atendentes poderão visualizar a fila de atendimento, assumir chamados, registrar interações, atualizar seus status e documentar as soluções realizadas.

O WantWeb terá como referência conceitos de sistemas de atendimento e contact center, adaptados a um projeto acadêmico com foco em organização, facilidade de uso e acompanhamento do ciclo de vida dos chamados.

### 1.3 Público-alvo

O WantWeb será destinado a organizações e equipes que necessitam organizar e acompanhar solicitações de atendimento por meio de chamados.

O sistema terá como principais usuários:

**Solicitante:** usuário que necessita de suporte e utiliza o sistema para abrir chamados, acompanhar o andamento das solicitações, enviar informações e consultar a solução.

**Atendente:** profissional responsável pelo atendimento dos chamados. Poderá visualizar a fila de atendimento, assumir solicitações, interagir com os solicitantes, atualizar o status e registrar a solução.

**Administrador:** usuário responsável pelo gerenciamento do sistema, podendo administrar usuários, categorias, prioridades e consultar informações dos chamados.

O sistema será desenvolvido inicialmente com foco em equipes de pequeno e médio porte que necessitam de uma ferramenta simples para organização do atendimento.

### 1.4 Requisitos Funcionais

Os requisitos funcionais descrevem as funcionalidades que o sistema deverá disponibilizar aos seus usuários.

**RF01 — Cadastro de usuários:** o sistema deverá permitir o cadastro de usuários.

**RF02 — Login:** o sistema deverá permitir que os usuários realizem autenticação por meio de login e senha.

**RF03 — Controle de acesso:** o sistema deverá permitir diferentes níveis de acesso de acordo com o perfil do usuário.

**RF04 — Abertura de chamado:** o sistema deverá permitir que o solicitante registre um novo chamado.

**RF05 — Número de protocolo:** o sistema deverá gerar um número de protocolo único para cada chamado.

**RF06 — Informações do chamado:** o sistema deverá permitir informar título, descrição, categoria e prioridade.

**RF07 — Consulta de chamados:** o solicitante deverá poder consultar os chamados que registrou.

**RF08 — Fila de atendimento:** o atendente deverá poder visualizar os chamados disponíveis para atendimento.

**RF09 — Atribuição de chamado:** o atendente deverá poder assumir um chamado para realizar o atendimento.

**RF10 — Atualização de status:** o sistema deverá permitir alterar o status do chamado durante seu ciclo de atendimento.

**RF11 — Interação no chamado:** o sistema deverá permitir o registro de mensagens entre solicitante e atendente.

**RF12 — Histórico:** o sistema deverá armazenar o histórico das interações e alterações realizadas no chamado.

**RF13 — Registro da solução:** o atendente deverá poder registrar a solução aplicada ao chamado.

**RF14 — Encerramento:** o sistema deverá permitir o encerramento de chamados após a resolução da solicitação.

**RF15 — Pesquisa e filtros:** o sistema deverá permitir pesquisar e filtrar chamados por informações como protocolo, status, prioridade e categoria.

**RF16 — Administração de usuários:** o administrador deverá poder cadastrar, consultar, alterar e desativar usuários.

**RF17 — Gerenciamento de categorias:** o administrador deverá poder cadastrar e gerenciar categorias de chamados.

**RF18 — Relatórios:** o sistema deverá permitir a consulta de informações básicas sobre os chamados e atendimentos realizados.

### 1.5 Requisitos Não Funcionais

Os requisitos não funcionais definem características de qualidade, segurança, desempenho, tecnologia e facilidade de utilização do sistema.

**RNF01 — Tecnologia:** o sistema deverá ser desenvolvido utilizando PHP.

**RNF02 — Banco de dados:** o sistema deverá utilizar MySQL para armazenamento das informações.

**RNF03 — Ambiente web:** o sistema deverá ser acessível por meio de um navegador web.

**RNF04 — Segurança:** o sistema deverá realizar autenticação dos usuários por meio de login e senha.

**RNF05 — Senhas:** as senhas dos usuários deverão ser armazenadas de forma segura, utilizando mecanismo de hash.

**RNF06 — Controle de acesso:** o sistema deverá restringir o acesso às funcionalidades de acordo com o perfil do usuário.

**RNF07 — Usabilidade:** a interface deverá ser simples, intuitiva e facilitar a realização das principais tarefas.

**RNF08 — Responsividade:** a interface deverá se adaptar a diferentes tamanhos de tela, como computadores, tablets e dispositivos móveis.

**RNF09 — Validação:** o sistema deverá validar os dados inseridos pelos usuários antes de realizar o processamento.

**RNF10 — Mensagens:** o sistema deverá apresentar mensagens claras de confirmação, alerta e erro.

**RNF11 — Manutenibilidade:** o código deverá ser organizado de forma a facilitar sua manutenção e evolução.

**RNF12 — Integridade:** o sistema deverá preservar a integridade e consistência dos dados armazenados.

**RNF13 — Histórico:** as informações relacionadas ao atendimento deverão permanecer registradas para consulta posterior.

**RNF14 — Desempenho:** as principais operações do sistema deverão apresentar tempo de resposta adequado para a utilização pelos usuários.

### 1.6 Regras de Negócio

As regras de negócio definem as condições e restrições que deverão ser respeitadas pelo WantWeb durante o funcionamento do sistema.

**RN01 — Protocolo único:** todo chamado deverá receber um número de protocolo único no momento de sua criação.

**RN02 — Campos obrigatórios:** um chamado somente poderá ser aberto quando os campos obrigatórios estiverem preenchidos.

**RN03 — Status inicial:** todo chamado criado deverá iniciar com o status **ABERTO**.

**RN04 — Fila de atendimento:** chamados com status **ABERTO** deverão permanecer disponíveis na fila de atendimento até que um atendente os assuma.

**RN05 — Atendimento:** somente um atendente poderá assumir um chamado para realizar seu atendimento.

**RN06 — Status em atendimento:** quando um atendente assumir um chamado, o status poderá ser alterado para **EM ATENDIMENTO**.

**RN07 — Aguardando usuário:** quando o atendimento depender de uma informação do solicitante, o chamado poderá receber o status **AGUARDANDO USUÁRIO**.

**RN08 — Retorno do solicitante:** quando o solicitante fornecer a informação necessária, o chamado poderá retornar para **EM ATENDIMENTO**.

**RN09 — Solução:** o chamado deverá possuir uma solução registrada antes de ser encerrado.

**RN10 — Encerramento:** somente chamados que tenham sido solucionados poderão ser encerrados.

**RN11 — Histórico:** alterações de status, mensagens e informações relevantes do atendimento deverão permanecer registradas no histórico.

**RN12 — Permissões:** cada usuário poderá executar somente as ações permitidas para seu perfil de acesso.

**RN13 — Solicitante:** o solicitante poderá visualizar e interagir somente com os chamados aos quais possui acesso.

**RN14 — Atendente:** o atendente poderá visualizar os chamados disponíveis para atendimento e aqueles que estiverem sob sua responsabilidade.

**RN15 — Administrador:** o administrador poderá gerenciar usuários, categorias e configurações permitidas pelo sistema.

**RN16 — Prioridade:** cada chamado deverá possuir uma classificação de prioridade para auxiliar na organização da fila de atendimento.

**RN17 — Integridade:** um chamado não poderá ser excluído de forma que seu histórico de atendimento seja perdido.

### 1.7 Escopo

O escopo do WantWeb compreende o desenvolvimento de um sistema web para gerenciamento de chamados, contemplando as principais etapas do ciclo de atendimento, desde a abertura da solicitação até sua resolução e encerramento.

#### Funcionalidades dentro do escopo

- Cadastro e gerenciamento de usuários.
- Autenticação por login e senha.
- Controle de acesso por perfil.
- Abertura de chamados.
- Geração de protocolo único.
- Cadastro e seleção de categorias.
- Classificação de prioridade.
- Visualização de chamados.
- Organização dos chamados em fila de atendimento.
- Atribuição de chamados aos atendentes.
- Atualização dos status dos chamados.
- Troca de mensagens entre solicitante e atendente.
- Registro do histórico de atendimento.
- Registro da solução.
- Encerramento dos chamados.
- Pesquisa e filtros de chamados.
- Relatórios básicos de atendimento.

#### Funcionalidades fora do escopo inicial

Para manter o projeto adequado ao escopo acadêmico e possibilitar a entrega de um MVP funcional, não serão implementados inicialmente:

- Atendimento por telefone ou VoIP.
- Integração com WhatsApp.
- Chatbot.
- Inteligência artificial para atendimento.
- Integração com redes sociais.
- Integração com sistemas ERP ou CRM externos.
- Atendimento omnichannel.
- Automação avançada de distribuição de chamados.
- Aplicativo mobile nativo.

Essas funcionalidades poderão ser consideradas como possibilidades de evolução futura do sistema.

#### Limitações do projeto

O WantWeb será desenvolvido inicialmente como um projeto acadêmico, utilizando PHP e MySQL, com foco no gerenciamento básico do ciclo de vida dos chamados e na aplicação dos conceitos de análise de requisitos, UX/UI, banco de dados, desenvolvimento web, controle de versões e testes de software.

### 1.8 Fluxo do Chamado

O ciclo de vida de um chamado no WantWeb será composto por etapas que representam o andamento da solicitação desde sua abertura até o encerramento.

#### Etapas do fluxo

**1. Abertura do chamado**

O solicitante acessa o sistema, preenche as informações necessárias e registra uma nova solicitação. Após o cadastro, o sistema gera um número de protocolo único.

**2. Status ABERTO**

Após sua criação, o chamado recebe o status **ABERTO** e fica disponível na fila de atendimento.

**3. Atendimento**

Um atendente visualiza a fila e assume o chamado. O status é alterado para **EM ATENDIMENTO**.

**4. Aguardando usuário**

Caso seja necessária alguma informação adicional do solicitante, o atendente poderá alterar o status para **AGUARDANDO USUÁRIO**.

**5. Retorno ao atendimento**

Após o solicitante fornecer as informações necessárias, o chamado poderá retornar para o status **EM ATENDIMENTO**.

**6. Resolução**

Quando o problema ou solicitação for solucionado, o atendente deverá registrar a solução e alterar o status para **RESOLVIDO**.

**7. Encerramento**

Após a solução, o chamado poderá ser encerrado, passando para o status **ENCERRADO**.

#### Representação do fluxo

ABERTURA
   ↓
ABERTO
   ↓
EM ATENDIMENTO
   ↓
AGUARDANDO USUÁRIO
   ↓
EM ATENDIMENTO
   ↓
RESOLVIDO
   ↓
ENCERRADO

### 1.9 Funcionalidades previstas para o MVP

O MVP (Produto Mínimo Viável) do WantWeb será composto pelas funcionalidades essenciais para demonstrar o funcionamento do sistema de gerenciamento de chamados.

O objetivo do MVP é disponibilizar uma primeira versão funcional do sistema, permitindo validar o fluxo principal de atendimento antes da implementação de funcionalidades mais avançadas.

#### Funcionalidades do MVP

- Cadastro de usuários.
- Login e autenticação.
- Controle de acesso por perfil.
- Abertura de chamados.
- Geração automática de número de protocolo.
- Cadastro e seleção de categorias.
- Definição de prioridade do chamado.
- Visualização dos chamados.
- Fila de atendimento.
- Atribuição de chamados aos atendentes.
- Alteração do status do chamado.
- Troca de mensagens entre solicitante e atendente.
- Registro do histórico do atendimento.
- Registro da solução aplicada.
- Encerramento do chamado.
- Pesquisa e filtros básicos de chamados.

#### Perfis contemplados no MVP

**Solicitante**
- Realizar login.
- Abrir chamados.
- Consultar seus chamados.
- Acompanhar o status.
- Enviar mensagens.
- Consultar a solução e o encerramento.

**Atendente**
- Realizar login.
- Visualizar a fila de chamados.
- Assumir chamados.
- Atender solicitações.
- Alterar o status.
- Enviar mensagens.
- Registrar a solução.
- Encerrar chamados.

**Administrador**
- Realizar login.
- Cadastrar e gerenciar usuários.
- Gerenciar categorias.
- Consultar chamados.
- Acompanhar informações básicas do atendimento.

#### Fluxo principal do MVP

LOGIN
  ↓
ABERTURA DO CHAMADO
  ↓
GERAÇÃO DO PROTOCOLO
  ↓
FILA DE ATENDIMENTO
  ↓
ATENDENTE ASSUME
  ↓
EM ATENDIMENTO
  ↓
REGISTRO DA SOLUÇÃO
  ↓
RESOLVIDO
  ↓
ENCERRADO
