# Requisitos do produto

## 1. Visão geral

Este documento identifica requisitos esperados para o produto BR-lol. Como o projeto está em fase de planejamento, os itens abaixo devem ser entendidos como base de discussão e não como escopo final confirmado.

## 2. Status das exigências

- Confirmado: requisito claramente descrito no contexto do projeto.
- Proposto: hipótese funcional ou técnica que ainda precisa ser validada.
- Pendente: dependente de decisão de negócio, experiência do usuário ou arquitetura.

## 3. Requisitos funcionais

### 3.1 Currículos

- RF-01: permitir criação e edição de currículos. (Confirmado)
- RF-02: permitir importar conteúdos existentes para edição. (Confirmado)
- RF-03: permitir exportar currículo em formatos adequados ao uso profissional. (Confirmado)
- RF-04: suportar múltiplos modelos de currículo. (Confirmado)
- RF-05: permitir adaptação do currículo para uma vaga específica. (Confirmado)
- RF-06: oferecer análise de compatibilidade com ATS. (Confirmado)
- RF-07: sugerir melhorias de conteúdo com base em critérios profissionais. (Proposto)

### 3.2 Bewrite

- RF-08: corrigir erros gramaticais e de estilo. (Confirmado)
- RF-09: reescrever textos mantendo intenção original. (Confirmado)
- RF-10: adaptar textos para diferentes contextos de candidatura. (Confirmado)
- RF-11: permitir tradução ou recontextualização de textos. (Confirmado)
- RF-12: preservar informações essenciais ao realizar reescrita. (Confirmado)

### 3.3 Quadro visual

- RF-13: permitir organização visual de ideias e processos. (Confirmado)
- RF-14: criar diagramas e mapas mentais. (Confirmado)
- RF-15: apoiar organização de candidaturas e etapas de processo. (Confirmado)
- RF-16: permitir estruturação de fluxo de trabalho e tarefas. (Proposto)

## 4. Requisitos não funcionais

- RNF-01: a experiência deve ser simples e clara. (Confirmado)
- RNF-02: o sistema deve permitir manutenção e evolução incremental. (Confirmado)
- RNF-03: a documentação deve acompanhar mudanças de produto e arquitetura. (Confirmado)
- RNF-04: a aplicação deve tratar dados pessoais com responsabilidade. (Confirmado)
- RNF-05: a solução deve permitir escalabilidade de módulos sem quebra de arquitetura. (Proposto)
- RNF-06: o projeto deve prever requisitos de acesso, auditoria e segurança para conteúdo sensível. (Pendente)

## 5. Requisitos de segurança

- uso de controle de acesso apropriado para dados pessoais;
- proteção de conteúdo do usuário e informações de carreira;
- cifragem e controle de arquivos exportados;
- políticas claras de retenção e privacidade.

## 6. Dependências e riscos

### Dependências

- definição de público-alvo e prioridade de módulos;
- decisão de plataforma e stack principal;
- estratégia para armazenamento de documentos e perfis;
- definição de autenticação e autorização;
- escolha de mecanismos de IA, se aplicável.

### Riscos

- escopo amplo demais para uma primeira entrega;
- ambiguidade entre módulos e prioridade funcional;
- uso de IA sem governança clara;
- necessidade de dados pessoais sem política de segurança estabelecida;
- múltiplas modalidades de exportação e edição sem padrão definido.

## 7. Itens pendentes de decisão

- qual módulo deve entrar primeiro no MVP;
- quais integrações são essenciais no primeiro ciclo;
- o produto será focado em web ou multi-plataforma;
- como documentos e textos serão armazenados;
- qual nível de automação de IA será aceito;
- quais regras de privacidade e conformidade devem ser atendidas.

## 8. Resumo

Os requisitos do BR-lol estão alinhados ao contexto de um produto prático para carreira profissional, mas ainda precisam ser refinados para definir a prioridade inicial de desenvolvimento, modelo de dados, arquitetura técnica e política de segurança.
