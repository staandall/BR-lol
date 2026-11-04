# Proposta de arquitetura

## 1. Objetivo

Este documento define uma proposta inicial de arquitetura para o BR-lol, sem caráter definitivo. A intenção é estabelecer uma base coerente para discussão e evolução posterior, mantendo simplicidade e clareza.

## 2. Princípios

- manter o produto modular;
- separar domínios por responsabilidade;
- facilitar evolução por módulo;
- reduzir acoplamento inicial;
- preservar capacidade de expansão sem introduzir complexidade prematura;
- documentar decisões como propostas, não como escolhas definitivas.

## 3. Visão geral da arquitetura proposta

A estrutura sugerida é uma arquitetura por módulos com fronteiras de domínio bem definidas:

- camada de apresentação;
- camada de aplicação/serviços de domínio;
- camada de infraestrutura e integrações;
- camada de persistência e armazenamento de conteúdo;
- camada de observabilidade e governança.

## 4. Domínios principais

### 4.1 Currículos

Responsável por:

- criação e edição de currículos;
- templates e modelos;
- exportação e importação;
- compatibilidade ATS;
- adaptação para vagas.

### 4.2 Bewrite

Responsável por:

- correção textual;
- reescrita de documentos;
- tradução e adaptação de linguagem;
- preservação de intenção e informação original.

### 4.3 Quadro visual

Responsável por:

- diagramas;
- mapas mentais;
- organização de processos;
- visualização de candidatura e fluxo de trabalho.

## 5. Organização sugerida

A arquitetura pode seguir uma estrutura como:

- `app/` — experiência de usuário e interface;
- `core/` — regras de negócio centrais;
- `modules/curriculum/` — domínio de currículo;
- `modules/bewrite/` — domínio de revisão e adaptação;
- `modules/board/` — domínio visual e de organização;
- `shared/` — utilitários, modelos e componentes reutilizáveis;
- `services/` — integrações externas e processamento assíncrono;
- `storage/` — persistência e arquivos do usuário;
- `security/` — autenticação, autorização e proteção de dados.

## 6. Proposta de implantação

A opção mais conservadora para o início é:

- arquitetura modular em um único projeto ou em monorepo bem organizado;
- separação por domínio para evitar acoplamento indevido;
- evolução gradual para serviços independentes apenas quando houver necessidade comprovada.

Essa abordagem reduz complexidade inicial e mantém controle sobre manutenção do produto.

## 7. Tecnologias e padrões sugeridos

Como o repositório ainda não contém implementação, a escolha tecnológica é aberta. O que está proposto é:

- frontend moderno e responsivo para web;
- APIs bem definidas para cada módulo;
- persistência leve e escalável conforme volume de dados;
- mecanismos de processamento para texto, documentos e exportação;
- gestão de arquivos e metadados; 
- observabilidade básica: logs, erros e métricas.

## 8. Riscos e considerações

- arquitetura ampla demais pode gerar complexidade desnecessária;
- módulos com dependências cruzadas podem gerar acoplamento;
- IA e geração de texto exigem governança clara;
- arquivos de documentos precisam de políticas claras de armazenamento e retenção;
- requisitos de autenticação e privacidade devem ser definidos antes de implementação completa.

## 9. Decisão proposta

A decisão técnica proposta é adotar um modelo modular com acoplamento baixo e evolução gradual, priorizando clareza e manutenção antes de especialização em microsserviços ou sistemas distribuídos complexos.

## 10. Itens pendentes

- decidir se o MVP será monolítico modular ou multi-serviço;
- definir stack de frontend e backend;
- definir como os conteúdos serão armazenados;
- decidir como o módulo de IA será integrado;
- validar caso de uso principal para início do desenvolvimento.
