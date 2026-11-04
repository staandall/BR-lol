# ADR-0001: arquitetura modular e incremental

- Status: Proposto
- Data: 2026-11-04

## Contexto

O projeto BR-lol abrange múltiplos módulos com objetivos e necessidades diferentes: currículo, revisão de texto e quadro visual. Em um estágio inicial, o principal risco é criar uma arquitetura excessivamente complexa antes que os requisitos e fluxos reais sejam confirmados.

## Decisão proposta

Adotar uma arquitetura modular com fronteiras de domínio bem definidas, mantendo a implementação inicial em uma estrutura simples, organizável e evolutiva. A separação por módulo deve ocorrer em nível de domínio, não necessariamente por serviço externo independente.

## Motivação

- reduzir acoplamento inicial;
- facilitar manutenção do código;
- permitir evolução em etapas;
- manter a capacidade de introduzir serviços específicos mais tarde, se houver necessidade.

## Consequências esperadas

### Positivas

- melhor organização por domínio;
- menor risco de fragilidade estrutural;
- mais clareza para novos colaboradores;
- evolução gradual sem reescrever todo o sistema.

### Negativas

- exige disciplina na separação de responsabilidades;
- pode exigir refatoração se o escopo crescer rapidamente;
- não resolve todos os problemas de produtividade sem mais entendimento do produto.

## Riscos e incertezas

- o módulo de IA pode exigir infraestrutura específica;
- requisitos de autenticação, armazenamento e organização de documentos ainda não foram definidos;
- a necessidade de sincronização entre módulos pode crescer com o tempo.

## Observação

Esta decisão é uma proposta inicial e não impede mudanças futuras. Caso a maturidade do produto exija, a arquitetura pode evoluir para uma abordagem mais distribuída ou mais especializada.
