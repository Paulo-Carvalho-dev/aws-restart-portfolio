# Modelo de Responsabilidade Compartilhada da AWS

## Introdução

A segurança é uma das principais prioridades da AWS. Para garantir ambientes seguros e confiáveis, a AWS adota o Modelo de Responsabilidade Compartilhada.

Nesse modelo, a segurança é dividida entre a AWS e o cliente, onde cada parte possui responsabilidades específicas sobre a proteção dos recursos e dados.

---

## Segurança DA Nuvem

A AWS é responsável pela segurança da infraestrutura que suporta todos os serviços disponibilizados na nuvem.

Isso inclui:

### Segurança Física

- Controle de acesso aos data centers
- Monitoramento contínuo
- Vigilância e proteção física
- Destruição segura de dispositivos de armazenamento

### Infraestrutura de Hardware

- Servidores
- Equipamentos de armazenamento
- Equipamentos de rede

### Infraestrutura de Software

- Sistemas utilizados para operar os serviços AWS
- Plataformas de virtualização

### Infraestrutura de Rede

- Roteadores
- Firewalls
- Balanceadores de carga
- Sistemas de detecção de intrusão

### Virtualização

- Isolamento entre instâncias
- Segurança da camada de virtualização

---

## Segurança NA Nuvem

O cliente é responsável por proteger tudo aquilo que implementa dentro da AWS.

Responsabilidades do cliente:

### Sistemas Operacionais

- Atualizações
- Correções de segurança (patches)
- Hardening do sistema

### Aplicações

- Desenvolvimento seguro
- Correções de vulnerabilidades
- Gerenciamento de credenciais

### Controle de Acesso

- Usuários IAM
- Perfis e permissões
- Políticas de segurança

### Configurações de Rede

- Security Groups
- Firewalls
- Regras de acesso

### Proteção de Dados

- Criptografia
- Controle de acesso
- Classificação dos dados

---

## Responsabilidades do Cliente Sobre os Dados

O cliente possui controle total sobre:

- Quais dados serão armazenados
- Onde esses dados serão armazenados
- Quem pode acessar os dados
- Como os dados serão protegidos
- Como os acessos serão concedidos ou removidos

---

## Responsabilidade Compartilhada por Modelo de Serviço

### IaaS (Infrastructure as a Service)

Exemplo:

- Amazon EC2

O cliente é responsável por:

- Sistema operacional
- Aplicações
- Atualizações
- Configuração de segurança

A AWS é responsável pela infraestrutura física.

---

### PaaS (Platform as a Service)

Exemplos:

- AWS Lambda
- Amazon RDS

A AWS gerencia:

- Infraestrutura
- Sistema operacional
- Plataforma

O cliente gerencia:

- Dados
- Permissões
- Configurações de acesso

---

### SaaS (Software as a Service)

Exemplos:

- AWS Trusted Advisor
- AWS Shield
- Amazon Chime

A AWS gerencia praticamente toda a infraestrutura e operação do serviço.

O cliente utiliza o serviço e gerencia apenas seus dados e acessos.

---

## Benefícios do Modelo de Responsabilidade Compartilhada

- Maior segurança
- Definição clara de responsabilidades
- Maior controle dos dados
- Redução de riscos operacionais
- Conformidade com boas práticas

---

## Conclusão

O Modelo de Responsabilidade Compartilhada define claramente quais aspectos da segurança são responsabilidade da AWS e quais permanecem sob responsabilidade do cliente. Compreender essa divisão é fundamental para construir ambientes seguros e operar corretamente recursos na nuvem.
