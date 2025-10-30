---
title: Docling Workshop - Lab 3
description: RAG multimodal con Docling
logo: images/DoclingDuck.png
---

# Lab 3: RAG multimodal con Docling

## 🎯 Objetivo

En este laboratorio combinarás todo lo aprendido para construir un sistema RAG (Retrieval Augmented Generation) completo y multimodal, potenciado con Docling.

## 📚 Lo que aprenderás

- Qué es RAG y cómo funciona
- Construir una base de conocimiento desde documentos
- Implementar búsqueda semántica con vectores
- Integrar modelos de lenguaje para generación
- Procesar y consultar contenido multimodal (texto + imágenes)
- Crear un sistema RAG verificable y transparente
- Usar modelos Granite a través de Replicate

## 🔄 ¿Qué es RAG?

[Retrieval Augmented Generation (RAG)](https://research.ibm.com/blog/retrieval-augmented-generation-RAG) es un patrón de aplicaciones de IA que mejora el rendimiento de los modelos de lenguaje al:

1. 🔍 **Recuperar**: Buscar información relevante en una base de conocimiento
2. 🔗 **Aumentar**: Añadir esa información al contexto del modelo
3. 💬 **Generar**: Producir respuestas basadas en información factual

### Beneficios de RAG

- ✅ **Respuestas más precisas**: Basadas en datos reales, no en memorización
- ✅ **Actualizable**: Añade nuevos documentos sin reentrenar el modelo
- ✅ **Verificable**: Puedes rastrear de dónde viene cada respuesta
- ✅ **Específico al dominio**: Usa tu propia base de conocimiento

### RAG Multimodal con Docling

Docling hace que RAG sea más potente al:

- 📄 Extraer texto estructurado de documentos complejos
- 🖼️ Procesar y entender imágenes en documentos
- 📊 Preservar tablas y gráficos con su contexto
- 🔗 Mantener relaciones entre elementos del documento

## Prerrequisitos

Este laboratorio es un [notebook de Jupyter](https://jupyter.org/). Sigue las instrucciones del [trabajo previo](../pre-work/README.md) para ejecutarlo.

## Lab

<!-- Con Replicate -->

[![# RAG multimodal con Docling - Replicate](https://badgen.net/badge/icon/github?icon=github&label=Ver%20en "Ver en GitHub")]({{ config.repo_url }}/blob/main/notebooks/Lab3_RAG.ipynb){:target="_blank"}
[![# RAG multimodal con Docling - Replicate](https://colab.research.google.com/assets/colab-badge.svg "Abrir en Colab")]({{ extra.colab_url }}/blob/main/notebooks/Lab3_RAG.ipynb){:target="_blank"}

<!-- Con LM Studio

[![# RAG multimodal con Docling - LM Studio](https://badgen.net/badge/icon/github?icon=github&label=Ver%20en "Ver en GitHub")]({{ config.repo_url }}/blob/main/notebooks/LM Studio RAG.ipynb){:target="_blank"}
[![# RAG multimodal con Docling - LM Studio](https://colab.research.google.com/assets/colab-badge.svg "Abrir en Colab")]({{ extra.colab_url }}/blob/main/notebooks/LM Studio RAG.ipynb){:target="_blank"} -->

Para ejecutar el notebook desde la línea de comandos en Jupyter usando el entorno virtual activo del [trabajo previo](../pre-work/README.md#instalar-jupyter), ejecuta:

```shell
jupyter notebook notebooks/Lab3_RAG.ipynb
```

La ruta del notebook anterior es relativa a la carpeta `docling-workshop` del repositorio de git clonado durante la sección de [preparación](../pre-work/README.md#clonar-el-repositorio-de-la-workshop-de-docling).