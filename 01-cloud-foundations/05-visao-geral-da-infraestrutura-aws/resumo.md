# Visão Geral da Infraestrutura da AWS

## Introdução

A infraestrutura global da AWS é composta por data centers distribuídos estrategicamente ao redor do mundo para fornecer alta disponibilidade, escalabilidade, desempenho e resiliência aos serviços em nuvem. 【1-3c73cf】

## Componentes da Infraestrutura Global

A infraestrutura da AWS é dividida em três componentes principais:

- Regiões (Regions)
- Zonas de Disponibilidade (Availability Zones)
- Pontos de Presença (Points of Presence) 【1-3c73cf】

---

## Data Centers AWS

Os Data Centers são a base física da infraestrutura da AWS.

Características:

- Armazenam os dados físicos dos clientes
- Realizam o processamento computacional
- Possuem entre 50.000 e 80.000 servidores físicos
- Permanecem sempre ativos
- Utilizam equipamentos de rede customizados pela AWS 【1-3c73cf】

### Recursos de Segurança

- Controle rigoroso de acesso
- Mitigação de riscos ambientais
- Arquitetura redundante
- Backup de componentes essenciais
- Desvio automático de tráfego em caso de falhas 【1-3c73cf】

---

## Zonas de Disponibilidade (Availability Zones)

Cada Zona de Disponibilidade é composta por um ou mais Data Centers fisicamente separados. 【1-3c73cf】

Características:

- Isolamento contra falhas
- Energia redundante
- Conectividade redundante
- Redes privadas de alta velocidade
- Baixa latência entre zonas 【1-3c73cf】

### Benefícios

- Maior disponibilidade
- Tolerância a falhas
- Resiliência contra desastres

A AWS recomenda distribuir aplicações entre múltiplas Zonas de Disponibilidade para aumentar a confiabilidade dos sistemas. 【1-3c73cf】

---

## Regiões AWS

Uma Região AWS corresponde a uma localização geográfica onde a AWS mantém múltiplas zonas de disponibilidade. 【1-3c73cf】

Características:

- Isolamento entre regiões
- Duas ou mais Availability Zones
- Controle manual de replicação entre regiões
- Atendimento a requisitos regulatórios e de conformidade 【1-3c73cf】

### Critérios para Seleção de Região

Ao escolher uma região é importante considerar:

- Latência
- Custos
- Requisitos legais
- Disponibilidade dos serviços
- Localização dos usuários finais 【1-3c73cf】

---

## Pontos de Presença (PoP)

Os Pontos de Presença são locais utilizados para aproximar os conteúdos da AWS dos usuários finais. 【1-3c73cf】

Atendem serviços como:

- Amazon CloudFront
- Amazon Route 53 【1-3c73cf】

Benefícios:

- Redução de latência
- Melhor experiência do usuário
- Distribuição global de conteúdo 【1-3c73cf】

---

## Características da Infraestrutura AWS

### Elasticidade

Capacidade de aumentar ou reduzir recursos automaticamente conforme a demanda. 【1-3c73cf】

### Escalabilidade

Permite o crescimento da infraestrutura à medida que o negócio evolui. 【1-3c73cf】

### Tolerância a Falhas

Capacidade de continuar operando mesmo diante de falhas em componentes individuais. 【1-3c73cf】

### Alta Disponibilidade

Projetada para minimizar períodos de indisponibilidade e garantir continuidade operacional. 【1-3c73cf】

---

## Conclusão

A infraestrutura global da AWS foi projetada para oferecer escalabilidade, disponibilidade, segurança e resiliência. O uso adequado de Regiões, Zonas de Disponibilidade e Pontos de Presença permite construir aplicações modernas capazes de atender usuários em escala global. 【1-3c73cf】
