# VPS-Compose

Este repositório contém uma configuração do Docker Compose para subir alguns serviços úteis em um ambiente de VPS.

## Serviços

O arquivo `docker-compose.yml` define os seguintes serviços:

- **cloudflaretunnel**: Cria um túnel seguro entre a sua VPS e a Cloudflare, permitindo expor serviços para a internet sem abrir portas no firewall.
- **postgres**: Um banco de dados relacional open-source.
- **pgadmin**: Uma ferramenta de administração para o PostgreSQL.
- **redis**: Um banco de dados em memória, geralmente usado para cache.
- **redisinsight**: Uma ferramenta de visualização e administração para o Redis.
- **filebrowser**: Um gerenciador de arquivos web, que permite acessar e gerenciar os arquivos da sua VPS através de uma interface web.

## Como usar

1. Clone este repositório.
2. Renomeie o arquivo `.env.sample` para `.env` e preencha as variáveis de ambiente.
3. Rode `docker-compose up -d` para subir os serviços.

## 🤝 Contribuição

Contribuições são bem-vindas! Se você tiver sugestões de melhorias, correções de bugs ou novas funcionalidades, sinta-se à vontade para abrir um pull request.

## 📊 Status do Projeto

![Status](https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow)

## 📄 Licença

Distribuído sob a licença MIT. Veja `LICENSE` para mais informações.

## 📧 Contato

Henrique Manduca - [LinkedIn](https://www.linkedin.com/in/henrique-manduca)