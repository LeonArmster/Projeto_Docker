# Projeto_Docker

**Data Criação:** 07/07/2025 <br>
**Autor:** Leonardo <br>
**Objetivo:** Esse projeto tem como objetivo aprender e aperfeiçoar a ferramenta Docker

### Primeiros passos:

Para utilização desse repositório faça os comandos abaixo:


**Clone o repositório**
```
git clone https://github.com/LeonArmster/Projeto_Docker.git
```

**Build a imagem**

```
docker build -t imagem-projeto
```

**Suba o container**
```
docker run -d -p 8501:8501 --name container-projeto imagem-projeto
```