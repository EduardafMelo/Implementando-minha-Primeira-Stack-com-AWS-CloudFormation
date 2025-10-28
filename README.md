# Implementando-minha-Primeira-Stack-com-AWS-CloudFormation

# 📝 Anotações - Laboratório AWS CloudFormation

Este repositório contém minhas **anotações detalhadas** durante a prática do laboratório **“Implementando sua Primeira Stack com AWS CloudFormation”**.  
Aqui registro tudo que aprendi, erros, soluções e insights importantes para referência futura.

---

## 1️⃣ Preparação do Ambiente

- Criar conta AWS ou usar conta existente.  
- Configurar permissões de **IAM** para criar stacks e recursos.  
- Abrir o console AWS ou CLI.  

**Dica:** Sempre verifique se você tem permissões suficientes antes de criar recursos.

---

## 2️⃣ Criando o Template

- Formato escolhido: **YAML**  
- Estrutura básica utilizada:

```yaml
AWSTemplateFormatVersion: '2010-09-09'
Description: 'Minha primeira stack'
Resources:
  MeuBucketS3:
    Type: AWS::S3::Bucket
    Properties:
      BucketName: meu-primeiro-bucket
