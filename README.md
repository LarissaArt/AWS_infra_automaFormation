# AWS_infra_automaFormation

# ☁️ AWS CloudFormation - Desafio Bootcamp Santander Code Girl DIO

Este repositório documenta minha experiência e aprendizados ao implementar uma **infraestrutura automatizada com AWS CloudFormation**, como parte do **bootcamp Santander Code Girl (DIO)**.  
Aqui compartilho **conceitos, práticas e reflexões** adquiridas durante o desafio.

---

## 🧠 O que é o AWS CloudFormation

O **AWS CloudFormation** é um serviço da Amazon Web Services que permite **criar, gerenciar e provisionar infraestrutura em nuvem** de forma **automatizada e segura**.  

Com **templates declarativos** em **YAML ou JSON**, você pode definir recursos como **EC2, S3, VPC, RDS**, entre outros — e o CloudFormation os organiza como um **único conjunto gerenciado, chamado *Stack***.

---

## 🚀 Benefícios do CloudFormation

| 💡 Benefício | 🌍 Descrição |
|---------------|---------------|
| **Automação** | Criação e atualização de infraestrutura sem ações manuais, garantindo consistência e evitando erros. |
| **Padronização** | Templates asseguram que todos os ambientes sigam a mesma configuração. |
| **Economia de custos** | Recursos podem ser criados e destruídos sob demanda, reduzindo desperdícios. |
| **Segurança** | Integra-se com **IAM**, garantindo permissões adequadas e políticas consistentes. |

---

## 🧩 Formatos de Template Suportados

O CloudFormation aceita dois formatos principais:

 **YAML (YAML Ain’t Markup Language)** → ✅ *Mais legível e fácil de manter.*  
 **JSON (JavaScript Object Notation)** → 🧱 *Mais rígido, porém compatível com automações antigas.*

---

## ⚙️ Fluxo de Criação da Stack

```yaml
flowchart LR
    A[📄 Template (YAML/JSON)] --> B[⚙️ AWS CloudFormation]
    B --> C[🔍 Validação e Interpretação]
    C --> D[🏗️ Criação da Stack]
    D --> E[☁️ Recursos AWS (EC2, S3, IAM...)]
    E --> F[✅ Infraestrutura Pronta e Gerenciada]
```

---

## 📘 Resumo do fluxo:

1- Template: descreve os recursos da infraestrutura.   

2- CloudFormation: interpreta o modelo e orquestra a criação.   

3- Stack: agrupa todos os recursos provisionados.  

---

## 🧠 CloudFormation x Terraform

| 🧾 **Característica** | ☁️ **CloudFormation** | 🧰 **Terraform** |
|------------------------|------------------------|------------------|
| **Provedor**           | AWS nativo             | Multi-cloud (AWS, Azure, GCP, etc.) |
| **Linguagem**          | YAML / JSON            | HCL (HashiCorp Configuration Language) |
| **Controle de estado** | Gerenciado automaticamente pela AWS | Manual ou remoto (`terraform.tfstate`) |
| **Escopo**             | Exclusivo da AWS       | Multi-cloud e serviços externos |

> 💬 **Resumo:** CloudFormation é ideal para projetos 100% AWS; Terraform é mais flexível para ambientes híbridos ou multi-cloud.


---

## 🛠️ Como criar uma Stack no CloudFormation

## 1- Crie ou use um template existente

*Defina os recursos (YAML ou JSON).

## 2- Armazene o template

*Localmente ou em um bucket S3.

## 3- Crie a Stack  

*Acesse o Console AWS CloudFormation.  

*Clique em "Create Stack" e selecione o template.  

*Configure parâmetros, permissões e opções.  

*Clique em "Create Stack" e acompanhe a criação.  

🔁 Após isso, o CloudFormation provisiona, atualiza ou exclui recursos conforme o template, mantendo controle de estado automaticamente.  

---

## 🏁 Conclusão   

O AWS CloudFormation é essencial no ecossistema DevOps por viabilizar Infraestrutura como Código (IaC) com automação, segurança, padronização e economia.  

Durante o bootcamp Santander Code Girl, foi possível compreender na prática como criar templates, gerenciar stacks e comparar ferramentas de IaC — consolidando fundamentos de Cloud Computing e DevOps.  

---

## 📚 Referências

📘 Documentação Oficial AWS CloudFormation

📄 Anatomia de Templates YAML - AWS Docs

🔗 Terraform vs CloudFormation - HashiCorp
