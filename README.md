# wantweb-sistema-chamados
Sistema web de gerenciamento de chamados desenvolvido em PHP e MySQL.
# WantWeb — Sistema de Gerenciamento de Chamados

## Sobre o projeto

O **WantWeb** é um sistema web de gerenciamento de chamados desenvolvido como projeto acadêmico.

O sistema tem como objetivo organizar o atendimento de solicitações, permitindo que usuários abram chamados e que atendentes acompanhem, assumam, atendam e encerrem essas solicitações.

O projeto utiliza conceitos de sistemas de atendimento e contact center, como **fila de atendimento, prioridade, status, atribuição de chamados e histórico**, adaptados para uma solução simples e acadêmica.

---

## Objetivo

Desenvolver uma solução web simples para registrar, organizar, acompanhar e controlar chamados desde sua abertura até o encerramento.

---

## Público-alvo

O sistema possui três perfis principais:

-  **Solicitante** — abre e acompanha seus chamados.
-  **Atendente** — realiza o atendimento e registra as soluções.
-  **Administrador** — gerencia usuários, categorias e informações do sistema.

---

##  Tecnologias

As tecnologias previstas para o desenvolvimento são:

-  PHP
-  MySQL
-  HTML5
-  CSS3
-  JavaScript
-  Git
-  GitHub
-  Figma

---

##  Principais funcionalidades

- Cadastro de usuários
- Login e autenticação
- Controle de acesso por perfil
- Abertura de chamados
- Geração de protocolo
- Categorias e prioridades
- Fila de atendimento
- Atribuição de chamados
- Atualização de status
- Comunicação entre solicitante e atendente
- Histórico de atendimento
- Registro da solução
- Encerramento de chamados
- Pesquisa e filtros

---

##  Fluxo do chamado

```text
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
