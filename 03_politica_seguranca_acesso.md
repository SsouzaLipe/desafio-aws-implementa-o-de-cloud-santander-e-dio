# Política de Segurança e Acesso – Abstergo Industries

## Objetivo
Estabelecer diretrizes de segurança para garantir confidencialidade, integridade e disponibilidade das informações armazenadas na Cloud AWS.

## Princípios de Segurança
- Princípio do menor privilégio
- Segregação de funções
- Auditoria contínua
- Proteção de dados sensíveis

## Controle de Acesso
- Uso do AWS IAM para gerenciamento de usuários e permissões
- Criação de grupos por função (TI, Financeiro, Operações)
- Proibição de uso de credenciais compartilhadas

## Segurança de Dados
- Criptografia de dados em repouso (S3, RDS e DynamoDB)
- Criptografia de dados em trânsito (HTTPS/TLS)
- Backups automáticos e versionamento de arquivos no S3

## Monitoramento e Auditoria
- Monitoramento de acessos e eventos via CloudWatch
- Logs de atividades administrativas
- Alertas para tentativas de acesso não autorizadas

## Boas Práticas
- Rotação periódica de credenciais
- Revisão semestral de permissões
- Uso de autenticação multifator (MFA) para usuários críticos

## Conformidade
Esta política apoia requisitos regulatórios comuns ao setor farmacêutico, como rastreabilidade, controle de acesso e auditoria de dados.
