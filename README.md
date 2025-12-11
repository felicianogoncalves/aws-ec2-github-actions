# AWS EC2 com GitHub Actions 🚀

Este repositório demonstra como criar e gerir uma instância **EC2 na AWS** utilizando **GitHub Actions** para automatizar o processo de provisionamento.

---

## 📌 Objetivo
- Automatizar a criação de uma instância EC2 na AWS.
- Usar **Infrastructure as Code (IaC)** através de workflows YAML.
- Mostrar integração entre **GitHub Actions** e **AWS**.

---

## ⚙️ Tecnologias utilizadas
- **AWS EC2** → serviço de máquinas virtuais na nuvem.
- **GitHub Actions** → CI/CD para automatizar o deploy.
- **YAML Workflows** → definição dos pipelines.


## 🚀 Como funciona
1. O workflow é acionado por **push** ou manualmente.
2. O GitHub Actions autentica na AWS usando **Secrets** configurados no repositório.
3. É criada uma instância EC2 com as especificações definidas no ficheiro `ec2.yml`.

---

## 🔐 Configuração necessária
Antes de correr o workflow, adiciona os seguintes **Secrets** no GitHub:
- `AWS_ACCESS_KEY_ID` → chave de acesso da tua conta AWS.
- `AWS_SECRET_ACCESS_KEY` → chave secreta da tua conta AWS.
- (Opcional) `AWS_REGION` → região onde a instância será criada (ex.: `us-east-1`).

---

## ▶️ Executar
- Faz um **push** para o branch principal (`main`) ou dispara manualmente o workflow.  
- O GitHub Actions vai provisionar automaticamente a instância EC2 na tua conta AWS.


## 👨‍💻 Autor
Projeto desenvolvido por Feliciano Gonçalves.
