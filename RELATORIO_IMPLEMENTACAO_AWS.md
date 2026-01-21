# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

Data: 20/01/2026  
Empresa: Abstergo Industries  
Responsável: Filipe Souza  

## Introdução
Este relatório apresenta o processo de implementação de serviços em Cloud Computing na empresa **Abstergo Industries**, realizado por **Filipe Souza**.  
O objetivo do projeto foi elencar **03 serviços AWS**, com foco principal em **redução imediata de custos operacionais**, aumento de escalabilidade e preparação da empresa para crescimento sustentável, considerando que atualmente a organização não possui nenhuma infraestrutura em Cloud.

A Abstergo Industries atua no ramo farmacêutico, revendendo produtos para outras empresas que fazem a comercialização ao cliente final, o que exige confiabilidade, rastreabilidade de dados, controle de estoque e disponibilidade dos sistemas.

## Descrição do Projeto
O projeto de implementação de Cloud foi dividido em **3 etapas**, cada uma endereçando um problema específico do cenário atual on-premises e contribuindo diretamente para a redução de custos.

---

### Etapa 1:
- **Ferramenta:** Amazon S3  
- **Foco da ferramenta:** Armazenamento de dados escalável e de baixo custo  
- **Descrição do caso de uso:**  
  O Amazon S3 será utilizado como repositório central de dados da Abstergo Industries, incluindo:
  - Documentos fiscais e regulatórios (lotes, notas, registros de conformidade)
  - Relatórios de vendas e distribuição
  - Backups de sistemas legados  

  **Redução de custo:**  
  - Elimina a necessidade de servidores locais para armazenamento
  - Modelo de pagamento por uso (pay-as-you-go)
  - Possibilidade de uso de camadas mais baratas (como armazenamento frio) para dados pouco acessados  

  **Processo de implementação:**  
  - Criação de buckets organizados por tipo de dado  
  - Definição de políticas de acesso (IAM)  
  - Migração gradual dos arquivos locais para o S3  

---

### Etapa 2:
- **Ferramenta:** Amazon RDS  
- **Foco da ferramenta:** Banco de dados relacional gerenciado  
- **Descrição do caso de uso:**  
  O Amazon RDS será utilizado para hospedar os bancos de dados transacionais da empresa, como:
  - Cadastro de clientes e distribuidores
  - Pedidos, faturamento e controle de estoque
  - Integração com sistemas ERP  

  **Redução de custo:**  
  - Elimina gastos com licenciamento, manutenção e administração de banco on-premises
  - Backup automático e alta disponibilidade nativos
  - Redução de horas de trabalho da equipe técnica com manutenção  

  **Processo de implementação:**  
  - Escolha do engine relacional adequado (ex: PostgreSQL ou MySQL)
  - Migração dos dados existentes
  - Configuração de backups automáticos e escalabilidade conforme demanda  

---

### Etapa 3:
- **Ferramenta:** Amazon DynamoDB  
- **Foco da ferramenta:** Banco de dados NoSQL de alta performance e baixa latência  
- **Descrição do caso de uso:**  
  O DynamoDB será utilizado para cenários que exigem alta velocidade e escalabilidade, como:
  - Rastreamento de pedidos em tempo quase real
  - Consulta rápida de status de entrega
  - Registro de eventos logísticos e movimentação de produtos  

  **Redução de custo:**  
  - Escalabilidade automática sem necessidade de superdimensionamento
  - Pagamento apenas pelas leituras e gravações realizadas
  - Elimina custos com servidores dedicados para picos de acesso  

  **Processo de implementação:**  
  - Modelagem das tabelas orientadas a chave
  - Integração com aplicações existentes
  - Definição de capacidade sob demanda  

---

## Conclusão
A implementação dos serviços **Amazon S3, Amazon RDS e Amazon DynamoDB** na empresa **Abstergo Industries** tem como principal objetivo a **redução imediata de custos operacionais**, aliada ao aumento de escalabilidade, segurança e disponibilidade dos sistemas.

O principal ganho dessa implementação é a **eliminação de investimentos em infraestrutura física**, permitindo que a empresa foque no seu core business, além de garantir flexibilidade para crescer de acordo com a demanda do mercado farmacêutico.

Recomenda-se a continuidade da adoção de serviços em Cloud, bem como a avaliação futura de ferramentas analíticas e de automação para otimizar ainda mais os processos internos da empresa.

## Anexos
- Documentação de arquitetura proposta  
- Plano de migração de dados  
- Política de segurança e acesso  

Assinatura do Responsável pelo Projeto:

Filipe Souza
