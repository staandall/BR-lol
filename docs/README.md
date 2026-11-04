# AGENTS.md

## Objetivo

Este repositório representa uma estrutura de produto em fase inicial de planejamento e documentação. A responsabilidade principal do desenvolvimento em andamento é manter clareza técnica, organização e rastreabilidade antes da implementação funcional.

## Regras gerais

- Não iniciar desenvolvimento de funcionalidades sem aprovação explícita.
- Não criar interfaces, componentes, páginas ou fluxos de produção.
- Não instalar dependências, ferramentas de terceiros ou bibliotecas sem justificativa técnica formal.
- Não configurar banco de dados, pagamentos, autenticação em produção, serviços externos ou credenciais.
- Não inventar requisitos que não estejam documentados no repositório.
- Registrar claramente o que está confirmado, proposto ou pendente de decisão.
- Proteger informações sensíveis: nunca expor segredos, tokens, chaves, dados pessoais ou credenciais.
- Não apagar arquivos existentes sem necessidade e sem justificativa técnica.
- Preservar histórico e conteúdo útil já presente no repositório.

## Prioridade de trabalho

1. Documentação de visão do produto.
2. Estrutura de requisitos e arquitetura.
3. Registro de decisões e riscos.
4. Planejamento em etapas e critérios de conclusão.
5. Apenas depois, implementação técnica real, se aprovada.

## Convenções de documentação

- Escrever em português brasileiro, de forma objetiva e técnica.
- Preferir clareza e precisão a textos genéricos.
- Diferenciar claramente entre:
  - Confirmado: requisito ou contexto já explícito.
  - Proposto: hipótese de solução ou arquitetura.
  - Pendente: decisão que ainda precisa ser confirmada.
- Usar a documentação da pasta `docs/` como fonte primária de consistentência.
- Mantém uma estrutura de projeto enxuta e profissional.

## Estrutura esperada

- `docs/README.md` — introdução à documentação.
- `docs/product/` — visão e requisitos do produto.
- `docs/architecture/` — arquitetura proposta e decisões técnicas.
- `docs/security/` — baseline de segurança.
- `docs/plan/` — roadmap e critérios de progresso.
- `docs/operations/` — procedimentos de manutenção do repositório.

## Comunicação e mudanças

- Qualquer alteração de arquitetura, requisitos ou escopo deve ser refletida na documentação antes de ser considerada válida.
- Mudanças importantes devem ser evidenciadas em documentos do tipo "decisão técnica" e não escondidas em commits isolados.
- Sempre que houver dúvida sobre objetivo, escopo ou prioridade, a resposta correta é reforçar a documentação existente antes de agir.

## Escopo de implementação permitido

Durante esta fase, o trabalho deve se limitar a:

- atualizar README principal;
- criar e manter documentos de contexto e planejamento;
- organiar a documentação técnica;
- registrar decisões técnicas e riscos;
- preparar roadmap e critérios de aceite.

Qualquer tarefa fora deste escopo deve ser tratada como pendente de aprovação.
