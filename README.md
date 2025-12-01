Lab - Docker: Utilização prática no cenário de Microsserviços
Atividade de Desafio do Bootcamp - Azure Advanced #2
Instrutor: Denilson Bonatti - Digital Innovation One

O projeto original é uma aplicacao monolítica que contem um Dockerfile, um nginx.conf, um index.php, um banco.sql (PHP + banco + servidor nginx)

A ideia original é replicar e melhorar o projeto prático, evoluindo para uma arquitetura de microsserviços em containers.

## Arquitetura

- API Gateway (NGINX)
- Microsserviços:
  - auth-service
  - catalog-service
  - cart-service
  - order-service
  - notification-service
- Cada serviço executa isolado em container
- Banco de dados por serviço (pattern: Database Per Service)
- Deploy com Azure Container Apps
- CI/CD com GitHub Actions

---

## Estrutura do Repositório

src/
api-gateway/
nginx.conf
Dockerfile
auth-service/
Dockerfile
catalog-service/
Dockerfile
cart-service/
Dockerfile
order-service/
Dockerfile
notification-service/
Dockerfile

docker/
docs/
.github/workflows/
docker-compose.yml
README.md


