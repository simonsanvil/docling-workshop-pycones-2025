---
title: Docling Workshop - Lab 3
description: RAG multimodal con Docling
logo: images/DoclingDuck.png
---

# RAG multimodal con Docling

[Retrieval Augmented Generation (RAG)](https://research.ibm.com/blog/retrieval-augmented-generation-RAG) es un patrón arquitectónico que puede utilizarse para mejorar el rendimiento de los modelos de lenguaje recuperando información factual de una base de conocimiento y añadiéndola a la consulta del modelo.

En este laboratorio combinaremos las habilidades aprendidas en los dos laboratorios anteriores para construir un sistema RAG potenciado con Docling.

## Prerrequisitos

Este laboratorio es un [notebook de Jupyter](https://jupyter.org/). Sigue las instrucciones del [trabajo previo](../pre-work/README.md) para ejecutarlo.

Este laboratorio tiene dos opciones de ejecución. La primera utiliza Replicate y la segunda usa LM Studio para ejecutarlo completamente en local.

## Lab

<!-- Con Replicate -->

[![# RAG multimodal con Docling - Replicate](https://badgen.net/badge/icon/github?icon=github&label=Ver%20en "Ver en GitHub")]({{ config.repo_url }}/blob/{{ git.commit }}/notebooks/RAG.ipynb){:target="_blank"}
[![# RAG multimodal con Docling - Replicate](https://colab.research.google.com/assets/colab-badge.svg "Abrir en Colab")]({{ extra.colab_url }}/blob/{{ git.commit }}/notebooks/RAG.ipynb){:target="_blank"}

<!-- Con LM Studio

[![# RAG multimodal con Docling - LM Studio](https://badgen.net/badge/icon/github?icon=github&label=Ver%20en "Ver en GitHub")]({{ config.repo_url }}/blob/{{ git.commit }}/notebooks/LM Studio RAG.ipynb){:target="_blank"}
[![# RAG multimodal con Docling - LM Studio](https://colab.research.google.com/assets/colab-badge.svg "Abrir en Colab")]({{ extra.colab_url }}/blob/{{ git.commit }}/notebooks/LM Studio RAG.ipynb){:target="_blank"} -->

Para ejecutar el notebook desde la línea de comandos en Jupyter usando el entorno virtual activo del [trabajo previo](../pre-work/README.md#instalar-jupyter), ejecuta:

```shell
jupyter notebook notebooks/RAG.ipynb
```

La ruta del archivo del notebook anterior es relativa a la carpeta `docling-workshop` del clonado de git en el [trabajo previo](../pre-work/README.md#clonar-el-repositorio-del-la-workshop-de-docling).