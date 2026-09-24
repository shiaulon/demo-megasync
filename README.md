# MegaSync EMP — Demonstração

Uma demonstração pública e interativa do **MegaSync EMP**, plataforma de gestão empresarial criada para centralizar operação, projetos, documentos, clientes e implantações.

## Acessar

**[Abrir a demonstração online](https://megasyncpitch-demo.web.app/)**

> A demo é uma cópia compilada do aplicativo Flutter, com dados fictícios. O acesso usa autenticação anônima no projeto Firebase separado megasyncpitch. Os dados de trabalho são criados no cache local do navegador, sem acesso ao Firestore de produção.

## Visão geral

O MegaSync organiza diferentes frentes de trabalho:

- **Painel Geral:** prioridades, prazos e indicadores operacionais;
- **CRM:** clientes, oportunidades e histórico;
- **Projetos:** quadros Kanban colaborativos;
- **Implantações:** ondas, etapas, subetapas e atividades;
- **GED:** documentos, assinatura, validação e comunicação;
- **Agenda:** compromissos consolidados dos demais módulos.

## Destaques

- Arquitetura multiempresa e permissões granulares;
- Atualizações em tempo real e interface responsiva;
- Integração entre operação, agenda, notificações e indicadores;
- Portais externos com acesso controlado;
- Integração ERP por API.

## Arquitetura

```mermaid
flowchart LR
  U[Usuários e clientes] --> A[Aplicação Flutter]
  A --> F[Firebase Auth]
  A --> D[Cloud Firestore]
  A --> S[Cloud Storage]
  A --> C[Cloud Functions]
  C --> E[ERP e serviços externos]
```

## Sobre este repositório

Este é um **repositório de apresentação**. O código-fonte proprietário do produto e o código de publicação da demo não fazem parte do repositório público. Aqui ficam apenas documentação e imagens autorizadas para portfólio.

O código-fonte da cópia demonstrativa permanece fora deste repositório público. O build é publicado separadamente no Firebase Hosting do projeto megasyncpitch. Recursos que dependem de serviços externos, como envio de arquivos e integrações, podem não funcionar na demo offline.

Desenvolvido por [Shiau Lon](https://github.com/shiaulon).
