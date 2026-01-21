# Documentação de Arquitetura Proposta – Abstergo Industries

## Visão Geral
Este documento descreve a arquitetura Cloud proposta para a empresa Abstergo Industries, com foco em redução de custos, escalabilidade, alta disponibilidade e segurança dos dados.

A arquitetura foi projetada considerando que a empresa não possui ambiente Cloud prévio e necessita de uma migração gradual, segura e de baixo impacto operacional.

## Arquitetura Geral
A solução é baseada em serviços gerenciados da AWS, reduzindo custos com infraestrutura física, licenciamento e manutenção.

### Componentes Principais
- Amazon S3: Armazenamento de arquivos, documentos e backups
- Amazon RDS: Banco de dados relacional transacional
- Amazon DynamoDB: Banco NoSQL para dados de alta performance
- AWS IAM: Controle de acesso e identidade
- AWS CloudWatch: Monitoramento e logs

## Fluxo de Dados
1. Sistemas internos e aplicações enviam dados transacionais para o Amazon RDS
2. Eventos operacionais e rastreamento de pedidos são registrados no DynamoDB
3. Documentos, relatórios e backups são armazenados no Amazon S3
4. Logs e métricas são monitorados via CloudWatch

## Justificativa da Arquitetura
- Redução de CAPEX com servidores físicos
- Alta disponibilidade nativa dos serviços AWS
- Escalabilidade automática conforme crescimento do negócio
- Pagamento sob demanda, reduzindo custos ociosos

## Considerações de Escalabilidade
- Amazon S3 e DynamoDB escalam automaticamente
- Amazon RDS pode ser escalado verticalmente conforme necessidade
- Arquitetura preparada para futura integração com analytics e BI
