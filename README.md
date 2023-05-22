# <p align = "center"> Projeto - Dockerfile Imagem Node  </p>

<p align="center">
   <img src="https://blog.geekhunter.com.br/wp-content/uploads/2019/06/docker-na-pratica-como-construir-uma-aplicacao-2.png"/>
</p>

<p align = "center">
   <img src="https://img.shields.io/badge/author-Januacele Vieira-4dae71?style=flat-square" />
   <img src="https://img.shields.io/badge/Learning - Docker -4dae71?style=flat-square" />
</p>

##  :clipboard: Descrição
  Esse projeto tem por finalidade mostrar o passo a passo da criação de um arquivo dockerfile que roda uma imagem do node. Ao fazer toda inicialização
  teremos um arquivo html rodando via container, sem usar os recursos de nossa máquina local.  
***
## :computer:	 Tecnologias e Conceitos

- Docker
- Dockerfile
- Imagem
- Container

## 🏁 Usando a Aplicação

Faça o clone desse repositório na sua maquina:

```
git clone git@github.com:Januacele/dockerfile-node.git
```
No seu terminal entre na pasta do projeto e rode o seguinte comando abaixo, definindo um nome para sua imagem. Pode ser qualquer nome, desde 
que seja escrito em minúsculo:

```
docker build -t + nome da imagem
```

Após criar a imagem, você pode ver todas as imagens listadas em seu container, com o comando:

```
docker images
```

Para rodar o projeto no servidor, defina as portas, nesse caso estamos usando como exemplo a porta 8080 que irá redirecionar para a 3000 (porta em que está
o nosso arquivo html):

```
docker run -p 8080:3000 + nome da imagem
```

Abra uma nova aba no seu navegador e digite:

```
http://localhost:8080
```

Assim, você terá criado um dockerfile que junta os arquivos do projeto, cria imagem node e sobe para um servidor num container docker. 
