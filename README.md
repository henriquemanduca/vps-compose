# VPS-Compose

![Status](https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow)

## Descrição

Crie esse repo para facilitar a configuração desses serviços em VPS particulares.

## Principais funcionalidades

O arquivo `docker-compose.yml` define os seguintes serviços:

- **Portainer-ce**: Edição comunitária do Portainer, uma ferramenta de gerenciamento de contêineres para Docker e Kubernetes.
- **Cloudflaretunnel**: Cria um túnel seguro entre a sua VPS e a Cloudflare, permitindo expor serviços para a internet sem abrir portas no firewall.
- **Postgresql**: Um banco de dados relacional open-source.
- **Pgadmin**: Uma ferramenta de administração para o PostgreSQL.
- **Redis**: Um banco de dados em memória, geralmente usado para cache.
- **Redisinsight**: Uma ferramenta de visualização e administração para o Redis.

## Tecnologias utilizadas

![Docker](https://img.shields.io/badge/docker-257bd6?style=for-the-badge&logo=docker&logoColor=white)

## Configuração

1. Renomeie o arquivo `.env.sample` para `.env` e preencha as variáveis de ambiente.
2. Rode `docker-compose up -d` para subir os serviços.

## Makefile

Este projeto inclui um `Makefile` para simplificar a atualização dos serviços Docker.

- Comando `update`:  Para atualizar um serviço específico, como o `Postgresql` ou `Redis`, utilize o comando `make update` com o parâmetro `service`. Este comando irá baixar a imagem mais recente do serviço e recriar o contêiner.
	- Exemplo: `$ make update service=Postgresql`
- comando  `help`: Para ver a lista de comandos disponíveis no `Makefile`.
	- Exemplo: `$ make help`

## Licença

Distribuído sob a licença MIT. Veja `LICENSE` para mais informações.

## Contato

- Henrique Manduca - [LinkedIn](https.linkedin.com/in/henrique-manduca)
- henriquemanduca@live.com