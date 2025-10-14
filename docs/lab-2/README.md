---
title: Docling Workshop - Lab 2
description: Chunking y vectorización con Docling
logo: images/DoclingDuck.png
---

# Chunking con Docling

El [chunking](https://www.ibm.com/architectures/papers/rag-cookbook/chunking) es el proceso de dividir textos largos en fragmentos más pequeños y manejables antes de pasarlos a un modelo. Es un paso importante porque los modelos tienen una longitud máxima de contexto, y el chunking se asegura que la información relevante quepa en ese límite, preservando la coherencia, mejorando la recuperación y evitando la pérdida de contenido importante durante el procesamiento.

En este laboratorio exploraremos la importancia del *chunking* y las capacidades que ofrece Docling para crear fragmentos de texto adecuados a la estructura y semántica del documento.

![docling-chunking](../images/chunking.png){: style="transform: scale(0.8); padding: 0px; margin: 0px;" }

## Prerrequisitos

Este laboratorio es un [notebook de Jupyter](https://jupyter.org/). Sigue las instrucciones del [trabajo previo](../pre-work/README.md) para ejecutarlo.

## Lab

[![# Chunking avanzado y vectorización con Docling - Notebook](https://badgen.net/badge/icon/github?icon=github&label=Ver%20en "Ver en GitHub")]({{ config.repo_url }}/blob/{{ git.commit }}/notebooks/Chunking.ipynb){:target="_blank"}
[![# Chunking avanzado y vectorización con Docling - Notebook](https://colab.research.google.com/assets/colab-badge.svg "Abrir en Colab")]({{ extra.colab_url }}/blob/{{ git.commit }}/notebooks/Chunking.ipynb){:target="_blank"}

Para ejecutar el notebook desde la línea de comandos en Jupyter usando el entorno virtual activo del [trabajo previo](../pre-work/README.md#instalar-jupyter), ejecuta:

```shell
jupyter notebook notebooks/Chunking.ipynb
```

La ruta del archivo del notebook anterior es relativa a la carpeta `docling-workshop` del clonado de git en el [trabajo previo](../pre-work/README.md#clonar-el-repositorio-de-la-workshop-de-docling).
