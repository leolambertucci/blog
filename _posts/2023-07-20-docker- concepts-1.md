---
title: "Conceitos Docker pt1 | Docker concepts pt1 - Image, Container, Engine"
date: 2023-07-20
tags:
- Docker
- Container
---

- Imagem (image):
  - Uma imagem é como uma captura de tela ou um modelo de um aplicativo de software e seu ambiente.
  - Ela contém todos os arquivos, bibliotecas e configurações necessários para executar o aplicativo.
  - As imagens são somente leitura e não podem ser modificadas; elas são usadas como um modelo para criar containers.
  - Você pode pensar em uma imagem como um pacote que contém tudo o que seu aplicativo precisa para ser executado.

- Container:
  - Um container é como uma instância em execução de uma imagem, criada a partir do modelo da imagem.
  - É um ambiente isolado e leve onde seu aplicativo é executado.
  - Os containers são como máquinas virtuais, mas eles compartilham o mesmo kernel do sistema operacional do host, tornando-os muito mais rápidos e eficientes.
  -Os containers são portáteis e podem ser executados consistentemente em diferentes ambientes.

- Docker Engine:
  - A engine é a tecnologia central que possibilita a existência e o funcionamento de containers.
  - O Docker Engine é uma implementação específica da tecnologia de containers.
  - Ele é responsável por criar e gerenciar containers com base em imagens.
  - Docker engine é executado na máquina host e interage com o sistema operacional para fornecer recursos de containers.
  -  O Docker Engine permite criar, executar e gerenciar containers usando comandos simples.
Resumo:
Em resumo, você pode pensar em uma imagem como um modelo ou pacote de um aplicativo, um container como uma instância em execução desse aplicativo, e o engine como a tecnologia que torna os containers possíveis e gerencia seu ciclo de vida.

Imagem: Modelo ou captura de tela de um aplicativo e seu ambiente.
container: Instância em execução de uma imagem; ambiente isolado onde o aplicativo é executado.
Docker Engine: Tecnologia central que possibilita containers, permitindo criar, executar e gerenciar containers.


---

- Image:
  - An image is like a snapshot or template of a software application and its environment.
  - It contains all the necessary files, libraries, and configurations needed to run the application.
  - Images are read-only and cannot be modified; they are used as a blueprint to create containers.
  - You can think of an image as a package that contains everything your application needs to run.
- Container:
  - A container is like a running instance of an image, created from the image template.
  - It is an isolated and lightweight environment where your application runs.
  - Containers are like virtual machines, but they share the same operating system kernel as the host, making them much faster and more efficient.
  - Containers are portable and can run consistently across different environments.
- Engine (Docker Engine):
  - The engine is the core technology that enables containers to exist and work.
  - Docker Engine is a specific implementation of containerization technology.
  - It is responsible for creating and managing containers based on images.
  - The engine runs on the host machine and interacts with the underlying operating system to provide container capabilities.
  - Docker Engine allows you to build, run, and manage containers using simple commands.

Summary:
In a nutshell, you can think of an image as a blueprint or package of an application, a container as a running instance of that application, and the engine as the technology that makes containers possible and manages their lifecycle.

Image: Template or snapshot of an application and its environment.
Container: Running instance of an image; isolated environment where the application runs.
Engine (Docker Engine): Core technology that enables containers, allowing you to create, run, and manage them.
