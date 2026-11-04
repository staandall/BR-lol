# Base de segurança

## 1. Objetivo

Estabelecer uma linha mínima de segurança para a evolução do BR-lol. Como o projeto ainda está em fase de planejamento, este documento define princípios e requisitos esperados, sem transformar decisões em implementação concluída.

## 2. Princípios

- minimizar coleta e armazenamento de dados desnecessários;
- proteger dados pessoais e informações de carreira;
- evitar exposição de segredos e credenciais;
- controlar acesso a conteúdo e documentos produzidos pelo usuário;
- manter políticas de retenção e recuperação claras.

## 3. Dados relevantes

O produto pode eventualmente lidar com:

- currículos e documentos profissionais;
- textos em diferentes línguas e contextos;
- preferências pessoais e histórico de candidatura;
- informação sensível sobre experiência profissional.

## 4. Requisitos mínimos esperados

- autenticação e autorização adequados para usuários e conteúdos;
- controle de acesso por identidade e papel;
- criptografia em trânsito para dados sensíveis;
- políticas de retenção definidas para documentos e arquivos;
- auditoria mínima para ações relevantes;
- proteção contra vazamento de segredos e chaves de sistema.

## 5. Riscos principais

- exposição indevida de currículos e dados pessoais;
- armazenamento de arquivos sem política de retenção;
- ausência de permissões claras em módulos compartilhados;
- vazamento de integrações com serviços externos;
- uso de IA sem políticas de privacidade e governança.

## 6. Decisões pendentes

- o produto será público ou privado por usuário;
- como os currículos serão armazenados e protegidos;
- haverá autenticação local, via provedor externo ou ambos;
- há necessidade de conformidade específica com dados pessoais;
- qual o nível de governança de IA será exigido.

## 7. Checklist de segurança para evolução

Antes de avançar para implementação, confirmar:

- não haverá segredos em arquivos públicos;
- todas as credenciais serão geridas por ambiente seguro;
- dados pessoais serão tratados com minimização e controle;
- acesso será granular por funcionalidade;
- fluxos de backup, recuperação e auditoria serão previstos.
