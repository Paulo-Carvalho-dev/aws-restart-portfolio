# Lab 01 - Amazon EC2

## Objetivo

Neste laboratório foi realizada a criação, configuração, monitoramento e gerenciamento de uma instância Amazon EC2 utilizando os recursos disponibilizados pelo ambiente AWS Academy/AWS re:Start.

O laboratório teve como foco a compreensão do ciclo de vida de uma instância EC2, além da configuração de segurança, armazenamento e monitoramento.

---

## Serviços Utilizados

- Amazon EC2
- Amazon EBS
- Security Groups
- Amazon CloudWatch
- Amazon VPC

---

## Atividades Realizadas

### 1. Criação da Instância

Foi criada uma instância EC2 utilizando:

- AMI Amazon Linux 2023
- Tipo de instância t3.micro
- Proteção contra encerramento habilitada
- Volume EBS padrão

---

### 2. Configuração do Servidor Web

Foi utilizado um script User Data para:

- Instalar o Apache HTTP Server
- Inicializar automaticamente o serviço
- Criar uma página HTML simples

Script utilizado:

```bash
#!/bin/bash
yum -y install httpd
systemctl enable httpd
systemctl start httpd
echo '<html><h1>Hello From Your Web Server!</h1></html>' > /var/www/html/index.html
```

---

### 3. Monitoramento

Foram analisados:

- Status Checks
- Métricas da instância
- Informações de monitoramento no CloudWatch

---

### 4. Configuração de Rede

Foi configurado um Security Group personalizado.

Inicialmente:

- Sem acesso HTTP

Posteriormente:

- Regra HTTP (porta 80)
- Origem: Anywhere IPv4

Permitindo acesso ao servidor web pela internet.

---

### 5. Redimensionamento

Foi realizado o redimensionamento da infraestrutura:

#### Instância

- Antes: t3.micro
- Depois: t3.small

#### Volume EBS

- Antes: 8 GiB
- Depois: 10 GiB

---

### 6. Proteção Contra Encerramento

Foi validado o funcionamento do recurso de proteção contra encerramento da instância.

Etapas:

1. Tentativa de encerramento bloqueada.
2. Desativação da proteção.
3. Encerramento da instância com sucesso.

---

## Resultados Obtidos

✅ Instância criada com sucesso

✅ Servidor Web implantado

✅ Security Group configurado

✅ Monitoramento realizado

✅ Instância redimensionada

✅ Proteção contra encerramento testada

✅ Instância encerrada corretamente

---

## Evidências

As capturas de tela encontram-se na pasta `evidencias`.

---

## Conhecimentos Aplicados

- Amazon EC2
- AMI
- User Data
- Security Groups
- Amazon EBS
- Amazon CloudWatch
- Escalabilidade Vertical
- Proteção contra Encerramento
- Administração de Instâncias
