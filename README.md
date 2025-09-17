 Validação de Arquivos com AWS Lambda

Este repositório documenta a implementação de uma função Lambda para validar arquivos enviados a um bucket S3. O objetivo é garantir que apenas arquivos com formato e tamanho adequados sejam processados, automatizando a triagem inicial de uploads.

 Descrição do Projeto

A função Lambda é acionada automaticamente quando um arquivo é enviado ao Amazon S3. Ela verifica:
- Tipo de arquivo (ex: `.pdf`, `.jpg`, `.csv`)
- Tamanho máximo permitido
- Presença de metadados obrigatórios

Arquivos inválidos são movidos para uma pasta de quarentena ou excluídos, conforme configuração.

Objetivos de Aprendizagem

- Criar funções Lambda com gatilho via S3
- Validar arquivos com base em regras definidas
- Registrar logs e erros via CloudWatch
- Documentar o processo técnico de forma clara

Tecnologias Utilizadas

- AWS Lambda
- Amazon S3
- Amazon CloudWatch
- AWS IAM
- Python 3.9
- GitHub + Markdown

Arquitetura da Solução

> Diagrama: S3 → Lambda → Validação → Ação (Mover/Excluir)  
> (Sugestão: incluir imagem na pasta `/images` com o fluxo)

Passo a Passo da Implementação

1. Criar bucket S3 com estrutura:
2. Desenvolver função Lambda em Python:
3. Configurar gatilho S3 → Lambda
4. Testar com arquivos válidos e inválidos
5. Ajustar permissões IAM

 Referências

- [Documentação AWS Lambda](https://docs.aws.amazon.com/lambda/)
- [Amazon S3 Event Notifications](https://docs.aws.amazon.com/AmazonS3/latest/userguide/EventNotifications.html)
- [Guia de Markdown no GitHub](https://guides.github.com/features/mastering-markdown/)

---
