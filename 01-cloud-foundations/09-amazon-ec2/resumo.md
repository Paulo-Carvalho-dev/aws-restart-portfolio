# Amazon EC2 (Elastic Compute Cloud)

## Introdução

O Amazon EC2 (Elastic Compute Cloud) é um dos principais serviços da AWS, fornecendo servidores virtuais seguros, escaláveis e sob demanda na nuvem.

Ele permite executar aplicações sem a necessidade de adquirir e manter infraestrutura física própria.

---

## Computação na AWS

A AWS oferece diferentes opções para execução de cargas de trabalho:

### Máquinas Virtuais

- Amazon EC2
- Amazon Lightsail

### Contêineres

- Amazon ECS
- Amazon EKS
- AWS Fargate

### Plataforma como Serviço (PaaS)

- AWS Elastic Beanstalk

### Computação Sem Servidor

- AWS Lambda
- AWS Fargate

### Soluções Especializadas

- AWS Outposts
- AWS Batch

Cada opção atende diferentes necessidades de desempenho, gerenciamento e escalabilidade.

---

## O que é Amazon EC2?

O Amazon EC2 fornece capacidade computacional na nuvem por meio de máquinas virtuais chamadas instâncias.

As instâncias podem ser utilizadas para:

- Servidores Web
- Servidores de Aplicação
- Bancos de Dados
- Jogos Online
- Servidores de Arquivos
- Processamento de Dados
- Aplicações Corporativas

---

## Significado de EC2

### Elastic

Capacidade de aumentar ou reduzir recursos conforme a demanda.

### Compute

Capacidade de processamento utilizando CPU e memória.

### Cloud

Infraestrutura hospedada na nuvem AWS.

---

## Benefícios do Amazon EC2

- Escalabilidade sob demanda
- Provisionamento rápido
- Pagamento conforme uso
- Alta disponibilidade
- Flexibilidade de configuração
- Integração com outros serviços AWS

---

## Sistemas Operacionais Suportados

O Amazon EC2 suporta diversos sistemas operacionais:

### Linux

- Amazon Linux
- Ubuntu
- Red Hat
- SUSE

### Windows

- Windows Server

---

## Amazon Machine Image (AMI)

Uma AMI (Amazon Machine Image) é um modelo utilizado para criar instâncias EC2.

Ela contém:

- Sistema Operacional
- Aplicações instaladas
- Bibliotecas
- Configurações

---

## Tipos de AMI

### Quick Start

Imagens disponibilizadas pela AWS.

### My AMIs

Imagens criadas pelo próprio usuário.

### AWS Marketplace

Imagens fornecidas por parceiros e fornecedores.

### Community AMIs

Imagens criadas pela comunidade.

---

## Benefícios das AMIs

### Repetibilidade

Permite criar diversas instâncias com a mesma configuração.

### Reutilização

Facilita a criação de ambientes padronizados.

### Recuperação

Permite recriar rapidamente servidores em caso de falhas.

---

## Tipos de Instância

Após escolher uma AMI, é necessário selecionar um tipo de instância.

Cada tipo possui combinações específicas de:

- CPU
- Memória
- Armazenamento
- Rede

---

## Categorias de Instâncias

### Uso Geral

Exemplo:

- Família T3

Indicadas para:

- Aplicações Web
- Ambientes de Desenvolvimento
- Microsserviços

### Otimizadas para Computação

Exemplo:

- Família C5

Indicadas para:

- Processamento intensivo
- Simulações
- Codificação de vídeo

### Otimizadas para Memória

Exemplo:

- Família R5

Indicadas para:

- Bancos de dados
- Big Data
- Cache distribuído

### Otimizadas para Armazenamento

Projetadas para aplicações com grande volume de dados.

### Computação Acelerada

Utilizam GPUs ou processadores especializados.

---

## Nomenclatura das Instâncias

Exemplo:

```text
t3.large
```

Onde:

- t = família da instância
- 3 = geração
- large = tamanho da instância

Em geral, gerações mais recentes oferecem melhor desempenho e custo-benefício.

---

## Rede e Conectividade

Ao criar uma instância é possível definir:

- Região AWS
- VPC
- Sub-rede
- Endereço IP Público
- Regras de Segurança

---

## Security Groups

Os Security Groups funcionam como firewalls virtuais.

Eles controlam:

- Tráfego de entrada
- Tráfego de saída
- Portas autorizadas
- Endereços permitidos

---

## Casos de Uso

### Hospedagem de Sites

Execução de aplicações web e APIs.

### Bancos de Dados

Execução de bancos relacionais e não relacionais.

### Processamento

Aplicações científicas e análises de dados.

### Ambientes Corporativos

Aplicações internas e sistemas empresariais.

### Desenvolvimento e Testes

Criação rápida de ambientes temporários.

---

## Conclusão

O Amazon EC2 é um dos serviços mais importantes da AWS, fornecendo capacidade computacional flexível, escalável e sob demanda. Sua integração com outros serviços da AWS permite criar arquiteturas modernas e altamente disponíveis para diferentes tipos de aplicações.
