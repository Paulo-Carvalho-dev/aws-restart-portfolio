# Redes na Nuvem AWS

## Introdução

As redes são um dos componentes fundamentais da computação em nuvem. Na AWS, o principal serviço responsável pela criação e gerenciamento de redes virtuais é o Amazon Virtual Private Cloud (Amazon VPC).

A Amazon VPC permite criar ambientes isolados dentro da infraestrutura da AWS, oferecendo controle sobre endereçamento IP, sub-redes, roteamento e segurança.

---

## O que é Amazon VPC?

O Amazon Virtual Private Cloud (Amazon VPC) é um serviço que permite criar uma rede virtual privada dentro da nuvem AWS.

Com uma VPC é possível:

- Definir intervalos de endereços IP.
- Criar sub-redes.
- Configurar tabelas de rotas.
- Controlar acessos através de regras de segurança.
- Conectar recursos à internet ou mantê-los isolados.

---

## Benefícios da Amazon VPC

- Isolamento lógico dos recursos.
- Segurança e controle de acesso.
- Escalabilidade.
- Flexibilidade na configuração da rede.
- Redução de custos com infraestrutura física.
- Facilidade para migração de ambientes tradicionais para a nuvem.

---

## Características da Amazon VPC

Uma VPC:

- Pertence a uma única Região AWS.
- Pode utilizar múltiplas Availability Zones.
- É logicamente isolada de outras VPCs.
- Permite implementação de arquiteturas seguras e escaláveis.

---

## Endereçamento IP e CIDR

Ao criar uma VPC é necessário definir um bloco CIDR (Classless Inter-Domain Routing).

Exemplo:

```text
10.0.0.0/16
```

A AWS permite blocos entre:

```text
/16 até /28
```

Os endereços devem utilizar faixas privadas definidas pela RFC 1918:

```text
10.0.0.0/8

172.16.0.0/12

192.168.0.0/16
```

---

## Componentes da Amazon VPC

### VPC

Rede virtual isolada na AWS.

### Sub-redes

Segmentações da rede principal.

Tipos:

- Sub-rede Pública
- Sub-rede Privada

---

### Gateway de Internet (IGW)

Permite comunicação entre recursos da VPC e a internet.

Características:

- Alta disponibilidade
- Escalabilidade automática
- Conectividade pública

---

### Gateway NAT

Permite que recursos em sub-redes privadas acessem a internet sem receber conexões iniciadas externamente.

Benefícios:

- Maior segurança
- Atualizações de sistemas
- Download de pacotes sem exposição pública

---

### Tabelas de Rotas

Controlam o direcionamento do tráfego da rede.

Uma rota possui:

#### Destino

Exemplo:

```text
0.0.0.0/0
```

#### Alvo

Exemplo:

```text
Internet Gateway
```

ou

```text
NAT Gateway
```

---

### Endpoint VPC

Permite comunicação privada entre recursos dentro da AWS sem utilizar a internet pública.

Benefícios:

- Maior segurança
- Menor latência
- Tráfego privado

---

## Sub-redes

### Sub-rede Pública

Possui rota para o Internet Gateway.

Permite:

- Servidores Web
- Load Balancers
- Recursos acessíveis pela internet

---

### Sub-rede Privada

Não possui acesso direto à internet.

Utilizada para:

- Bancos de Dados
- Aplicações internas
- Sistemas corporativos

---

## Segurança na VPC

### Security Groups

Firewall aplicado diretamente aos recursos.

Características:

- Stateful
- Controla tráfego de entrada e saída
- Bloqueia todo tráfego por padrão

---

### Network ACLs

Firewall aplicado na sub-rede.

Características:

- Stateless
- Regras de entrada e saída independentes
- Permite ou bloqueia tráfego

---

## Security Group vs Network ACL

| Recurso     | Security Group | Network ACL      |
| ----------- | -------------- | ---------------- |
| Localização | Instância      | Sub-rede         |
| Tipo        | Stateful       | Stateless        |
| Regras      | Permitir       | Permitir e Negar |
| Escopo      | Recurso        | Rede             |

---

## Arquitetura Básica de VPC

```text
Internet
    │
    ▼
Internet Gateway
    │
    ▼
Public Subnet
    │
    ├── EC2 Web Server
    │
Private Subnet
    │
    ├── Banco de Dados
    │
    ▼
NAT Gateway
```

---

## Conclusão

O Amazon VPC fornece os recursos necessários para criar redes seguras e escaláveis na AWS. O entendimento de VPCs, CIDR, sub-redes, roteamento e mecanismos de segurança é essencial para a construção de arquiteturas modernas em nuvem.
