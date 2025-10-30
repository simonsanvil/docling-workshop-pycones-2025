---
title: Docling Workshop - Lab 1
description: Conversión de documentos con Docling
logo: images/DoclingDuck.png
---

# Lab 1: Conversión de documentos con Docling

## 🎯 Objetivo

En este laboratorio aprenderás a usar Docling para convertir documentos complejos (PDFs, DOCX, PPTX) a formatos estructurados útiles para aplicaciones de IA.

## 📚 Lo que aprenderás

- Cómo instalar y configurar Docling
- Convertir diferentes tipos de documentos (PDF, DOCX, PPTX)
- Exportar a múltiples formatos (Markdown, JSON, HTML)
- Explorar la estructura de documentos convertidos
- Extraer y trabajar con metadatos de documentos
- Enriquecer documentos con OCR y análisis de imágenes

## 🔧 Funcionalidades de Docling que explorarás

El propósito principal de Docling es la conversión de documentos. Docling nos permite convertir documentos en diversos formatos a otros más útiles para aplicaciones de IA, preservando la estructura y contenido del documento.

### Formatos de entrada soportados
- PDF
- Microsoft Word (DOCX)
- Microsoft PowerPoint (PPTX)
- Imágenes (PNG, JPG)
- HTML
- Y más...

### Formatos de salida
- **Markdown**: Ideal para documentación y LLMs
- **JSON**: Perfecto para procesamiento programático
- **HTML**: Para visualización web
- **DoclingDocument**: Objeto Python con estructura completa

<!-- ![docling-conversion](../images/docling-banner.png) -->

## Prerrequisitos

Este laboratorio es un [notebook de Jupyter](https://jupyter.org/). Sigue las instrucciones del [trabajo previo](../pre-work/README.md) para ejecutarlo.

## Lab

[![Conversión de documentos con Docling - Notebook](https://badgen.net/badge/icon/github?icon=github&label=Ver%20en "Ver en GitHub")]({{ config.repo_url }}/blob/main/notebooks/Lab1_Docling_convert.ipynb){:target="_blank"}
[![Conversión de documentos con Docling - Notebook](https://colab.research.google.com/assets/colab-badge.svg "Abrir en Colab")]({{ extra.colab_url }}/blob/main/notebooks/Lab1_Docling_convert.ipynb){:target="_blank"}



Para ejecutar el notebook desde la línea de comandos en Jupyter usando el entorno virtual activo del [trabajo previo](../pre-work/README.md#instalar-jupyter), ejecuta:

```shell
jupyter notebook notebooks/Lab1_Docling_convert.ipynb
```

La ruta del notebook anterior es relativa a la carpeta `docling-workshop` del repositorio de git clonado durante la sección de [preparación](../pre-work/README.md#clonar-el-repositorio-de-la-workshop-de-docling).