# Meu Projeto DevOps

![CI](https://github.com/dumarie/meu-projeto-devops/actions/workflows/ci.yml/badge.svg)

Projeto prático desenvolvido durante o **Bootcamp DevOps 2026 (Instituto Matera)**, aplicando conteinerização, automação em Shell Script e integração contínua (CI) com GitHub Actions.

## 🛠️ Tecnologias Utilizadas

* **Linux (Ubuntu)** & **Shell Script** (automação de build, testes e healthcheck)
* **Docker** & **Docker Compose** (orquestração da aplicação web + banco em memória Redis)
* **Git** & **GitHub Actions** (pipeline automatizada de CI)

## 📂 Estrutura do Projeto

* `.github/workflows/ci.yml` — Pipeline de integração contínua (executa build e testes a cada `push` ou `pull_request` na `main`)
* `scripts/` — Scripts de automação (`build.sh`, `test.sh`, `deploy.sh` e monitoramento de `healthcheck`)
* `docs/` — Documentação complementar e certificado da formação
* `Dockerfile` — Definição da imagem customizada da aplicação
* `compose.yaml` — Orquestração dos serviços da aplicação e Redis

## 🚀 Como rodar

Clone o repositório e suba os contêineres com o Docker Compose:

```bash
git clone [https://github.com/dumarie/meu-projeto-devops.git](https://github.com/dumarie/meu-projeto-devops.git)
cd meu-projeto-devops
docker compose up -d
