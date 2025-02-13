# 🚀 1º Projeto Apache com Docker Compose

Este projeto consiste em rodar um **servidor Apache (httpd)** dentro de um **contêiner Docker**, utilizando **Docker Compose** para orquestrar o ambiente. A aplicação servida é uma simples página HTML.

## 📌 Como foi feito?
Todo o processo foi realizado **via comandos dentro do Docker Desktop**, o que ajudou a entender melhor a estrutura dos contêineres, volumes e serviços.

## 🛠️ Tecnologias Utilizadas:
- Docker 🐳
- Docker Compose 🛠️
- Apache HTTP Server 🌐
- HTML/CSS 💻

## 📂 Estrutura do Projeto:
```
📂 docker
 ├── 📂 html
 │    ├── index.html
 ├── docker-compose.yml
 ├── README.md
```

## 🚀 Como Rodar o Projeto:
1. **Clone o repositório** e entre na pasta `docker/`:
   ```sh
   git clone https://github.com/rodrigoalancelio/Jornada_DevOps_AWS.git
   cd Jornada_DevOps_AWS/docker
   ```
2. **Suba o ambiente com Docker Compose**:
   ```sh
   docker-compose up -d
   ```
3. **Acesse a aplicação no navegador**:
   ```
   http://localhost:8080
   ```
4. **Para parar o contêiner**:
   ```sh
   docker-compose down
   ```

## 📌 Aprendizados:
- Configuração de um ambiente Apache dentro do Docker.
- Uso de **volumes** para persistência de arquivos.
- Comandos essenciais do **Docker Compose**.

---
Agora é só subir o README no repositório! 🚀🔥

