# Amazon S3 (Simple Storage Service)

## Introdução

O Amazon S3 (Simple Storage Service) é o serviço de armazenamento de objetos da AWS. Ele permite armazenar arquivos de diferentes tipos, como documentos, imagens, vídeos, backups e logs de aplicações de forma escalável, segura e altamente durável.

---

## Conceitos Fundamentais

### Bucket

Um bucket é um contêiner lógico utilizado para armazenar objetos no Amazon S3.

Características:

- Cada bucket possui um nome único globalmente.
- Pode armazenar uma quantidade praticamente ilimitada de objetos.
- Permite definir permissões de acesso.
- Está associado a uma Região AWS específica.

### Objeto

Os arquivos armazenados no S3 são chamados de objetos.

Um objeto é composto por:

- Dados do arquivo
- Metadados
- Chave de identificação (Object Key)

Um objeto pode possuir até 5 TB de tamanho.

---

## Principais Características

### Alta Durabilidade

O Amazon S3 oferece durabilidade de:

- 99,999999999% (11 noves)

Os dados são armazenados de forma redundante em múltiplas instalações dentro da região escolhida.

### Escalabilidade

- Armazenamento praticamente ilimitado
- Crescimento automático
- Não exige provisionamento manual

### Segurança

- Dados privados por padrão
- Controle de acesso granular
- Criptografia opcional
- Suporte a HTTPS

### Disponibilidade

Os dados podem ser acessados de qualquer lugar através da internet.

---

## Classes de Armazenamento

### S3 Standard

Ideal para dados acessados frequentemente.

Casos de uso:

- Aplicações web
- Sites
- Distribuição de conteúdo
- Big Data

---

### S3 Intelligent-Tiering

Move automaticamente os dados entre camadas de armazenamento conforme os padrões de acesso.

Benefícios:

- Otimização de custos
- Gerenciamento automático

Ideal para dados com padrão de acesso imprevisível.

---

### S3 Standard-IA

(Infrequent Access)

Projetado para dados acessados ocasionalmente, mas que precisam estar disponíveis rapidamente.

Casos de uso:

- Backups
- Recuperação de desastres
- Arquivos de longa duração

---

### S3 One Zone-IA

Armazena os dados em apenas uma Availability Zone.

Benefícios:

- Menor custo

Indicado para:

- Dados recriáveis
- Backups secundários

---

### S3 Glacier

Classe de arquivamento de baixo custo.

Características:

- Armazenamento de longo prazo
- Tempo de recuperação maior
- Ideal para arquivamento

---

### S3 Glacier Deep Archive

Classe de armazenamento de menor custo da AWS.

Indicada para:

- Retenção de dados de longo prazo
- Compliance
- Arquivamento histórico

Tempo de recuperação pode chegar a até 12 horas.

---

## Redundância

Ao criar um bucket, os dados são armazenados de forma redundante em múltiplas instalações dentro da região selecionada.

Isso garante:

- Alta disponibilidade
- Tolerância a falhas
- Proteção contra perda de dados

---

## Casos de Uso

### Hospedagem de Sites Estáticos

Permite armazenar:

- HTML
- CSS
- JavaScript
- Imagens

### Backup

Armazenamento seguro para cópias de segurança.

### Big Data

Repositório para grandes volumes de dados utilizados em análises.

### Compartilhamento de Arquivos

Distribuição de conteúdos para aplicações e usuários finais.

### Recuperação de Desastres

Replicação entre regiões para recuperação em caso de falhas.

---

## Modelo de Precificação

O Amazon S3 utiliza o modelo Pay-As-You-Go.

Os custos são calculados com base em:

### Armazenamento

Quantidade de dados armazenados.

### Solicitações

Operações realizadas nos objetos.

Exemplos:

- GET
- PUT
- COPY
- LIST

### Transferência de Dados

Cobrança para tráfego de saída da região.

---

## Conclusão

O Amazon S3 é um dos serviços mais importantes da AWS, oferecendo armazenamento altamente durável, escalável e seguro. Sua variedade de classes de armazenamento permite equilibrar custo, desempenho e disponibilidade conforme a necessidade do negócio.
