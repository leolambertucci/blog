---
title: "Docker entrypoint"
date: 2023-07-20
tags:
- Docker
- Container
---

Pense nos containers Docker como pequenas máquinas virtuais que executam aplicativos específicos. Quando você inicia um container, ele precisa saber qual aplicativo vai executar dentro dele. É aí que entra o "entrypoint".

O entrypoint do Docker é como um comando padrão executado quando você inicia um container. Ele diz ao Docker qual deve ser a principal função do container.

Aqui está um exemplo para ajudar você a entender:

Suponha que você tenha um script Python simples chamado "hello.py" que imprime "Hello, Docker!" para o console.

Dockerfile:

Dockerfile
```Dockerfile
FROM python:3
COPY hello.py /app/hello.py
ENTRYPOINT ["python", "/app/hello.py"]
```

Crie e execute o container:

```bash
docker build -t my-container .
docker run my-container
```

Ao executar esse container, ele executará o script "hello.py" e você verá a saída:

```
Hello, Docker!
```

entrypoint do Docker:

- O entrypoint é como o comando padrão executado quando você inicia um container.
- Especifica o executável ou processo primário a ser executado dentro do container.
- O entrypoint é definido no Dockerfile usando a instrução ENTRYPOINT.
- O entrypoint não pode ser substituído ou alterado ao executar o container.


A principal diferença entre CMD e ENTRYPOINT no Docker é que, em termos de execução, os argumentos padrão fornecidos pelo CMD podem ser substituídos, enquanto os fornecidos pelo ENTRYPOINT não podem.


---

Think of Docker containers as little virtual machines that run specific applications. When you start a Docker container, it needs to know which application to run inside it. That's where the "entrypoint" comes in.

Docker entrypoint is like a default command that runs when you start a container. It tells Docker what should be the main thing the container does.

Here are some examples to help you understand:

Suppose you have a simple Python script called "hello.py" that prints "Hello, Docker!" to the console.

Dockerfile:

Dockerfile
```Dockerfile
FROM python:3
COPY hello.py /app/hello.py
ENTRYPOINT ["python", "/app/hello.py"]
```

Build and run the container:

```bash
docker build -t my-container .
docker run my-container
```

When you run this container, it will execute the "hello.py" script, and you'll see the output:

```
Hello, Docker!
```

Docker Entrypoint:

- The entrypoint is like the default command that runs when you start a container.
- It specifies the primary executable or process to run inside the container.
- The entrypoint is defined in the Dockerfile using the ENTRYPOINT instruction.
- The entrypoint cannot be overridden or changed when running the container.



The main difference between CMD and ENTRYPOINT in Docker is that, in terms of execution, the default arguments provided by CMD can be overridden, while those provided by ENTRYPOINT cannot.


