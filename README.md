# PyConES 2025 | Docling Workshop

[![Documentation](https://img.shields.io/badge/docs-mkdocs-blue)](https://simonsanvil.github.io/docling-workshop-pycones-2025/)
[![Python Version](https://img.shields.io/badge/python-3.10%20%7C%203.11%20%7C%203.12-blue)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Repositorio de la workshop de Docling presentado en la [PyConES 2025](https://2025.es.pycon.org/). Aquí encontrarás el material, documentación y notebooks prácticos usados durante la sesión.

## Enlaces rápidos

- 📚 **Documentación**: https://simonsanvil.github.io/docling-workshop-pycones-2025/
- 🦆 **Proyecto Docling**: https://docling-project.github.io/docling/
- 🐙 **Repositorio Original**: https://github.com/ibm-granite-community/docling-workshop

## ¿Qué vas a aprender?

Al finalizar esta workshop serás capaz de:
- Convertir documentos complejos a formatos útiles para IA preservando su estructura con Docling.
- Entender y aplicar técnicas de chunking y vectorización para mejorar tu sistema de recuperación de información.
- Construir un sistema RAG multimodal transparente y verificable.

## Contenido

La documentación completa de la workshop está en [docs/](/docs/) y publicada en el sitio anterior. Recomendamos seguir la navegación del sitio web publicado para una mejor experiencia.

La documentación se divide en las siguientes secciones:

- [Introducción](/docs/README.md): Una pequeña introducción a Docling y contenido de la workshop.
- [Preparación de entorno](/docs/pre-work/README.md): Instrucciones para preparar tu entorno de trabajo y ejecutar los notebooks.

Los tres notebooks prácticos donde se desarrolla la parte práctica de la workshop:

- [`Lab 1 – Conversión de documentos`](/docs/lab-1/README.md) [![Conversión de documentos con Docling - Notebook](https://colab.research.google.com/assets/colab-badge.svg "Abrir en Colab")](https://colab.research.google.com/github/simonsanvil/docling-workshop-pycones-2025/blob/main/notebooks/Lab1_Docling_convert.ipynb)
- [`Lab 2 – Chunking y vectorización`](/docs/lab-2/README.md) [![Chunking y vectorización con Docling - Notebook](https://colab.research.google.com/assets/colab-badge.svg "Abrir en Colab")](https://colab.research.google.com/github/simonsanvil/docling-workshop-pycones-2025/blob/main/notebooks/Lab2_Chunking.ipynb)
- [`Lab 3 – RAG multimodal`](/docs/lab-3/README.md) [![RAG multimodal con Docling - Notebook](https://colab.research.google.com/assets/colab-badge.svg "Abrir en Colab")](https://colab.research.google.com/github/simonsanvil/docling-workshop-pycones-2025/blob/main/notebooks/Lab3_RAG.ipynb)

Puedes abrirlos en local (ver sección de preparación) o ejecutarlos en Google Colab haciendo click en los badges correspondientes.

## Requisitos previos

- Git y Python 3.10, 3.11 o 3.12
- Cuenta en [Replicate](https://replicate.com/) para usar modelos de IA en la nube.
- Para ejecutar notebooks en local: Jupyter Notebook o JupyterLab

Consulta detalles y pasos en: [docs/pre-work/README.md](/docs/pre-work/README.md) (Preparación).

## Preparación rápida

### Para ejecutar los notebooks localmente

```bash
# 1. Clona el repositorio
git clone https://github.com/simonsanvil/docling-workshop-pycones-2025
cd docling-workshop-pycones-2025

# 2. Instala uv (si no lo tienes)
pip install uv

# 3. Instala dependencias
uv sync --no-dev

# 4. Abre los notebooks con Jupyter
jupyter notebook notebooks/
```

### Para servir la documentación localmente

```bash
# Instalar dependencias incluyendo las de desarrollo
uv sync --all-groups

# Servir la documentación en http://localhost:8000
uv run mkdocs serve
```

### Para usar Google Colab

Simplemente haz clic en los badges 🚀 de Colab en cada lab o ve directamente a:
- [Lab 1 en Colab](https://colab.research.google.com/github/simonsanvil/docling-workshop-pycones-2025/blob/main/notebooks/Lab1_Docling_convert.ipynb)
- [Lab 2 en Colab](https://colab.research.google.com/github/simonsanvil/docling-workshop-pycones-2025/blob/main/notebooks/Lab2_Chunking.ipynb)
- [Lab 3 en Colab](https://colab.research.google.com/github/simonsanvil/docling-workshop-pycones-2025/blob/main/notebooks/Lab3_RAG.ipynb)

Para preparación detallada (entornos, Jupyter, variables de entorno para Replicate, etc.), sigue los pasos en [docs/pre-work/README.md](/docs/pre-work/README.md).

## Construir la documentación

Para generar el sitio estático en `site/`:

```bash
uv run mkdocs build --clean
```

La documentación utiliza [MkDocs Material](https://squidfunk.github.io/mkdocs-material/) con algunas personalizaciones. El tema y configuración están en `mkdocs.yml`.

## Estructura del repositorio

```
docling-workshop-pycones-2025/
├── docs/                    # Documentación fuente (MkDocs)
│   ├── images/             # Imágenes de la documentación
│   ├── css/                # Estilos personalizados
│   ├── pre-work/           # Instrucciones de preparación
│   ├── lab-1/              # Lab 1: Conversión de documentos
│   ├── lab-2/              # Lab 2: Chunking y vectorización
│   └── lab-3/              # Lab 3: RAG multimodal
├── notebooks/              # Notebooks de los laboratorios
│   ├── Lab1_Docling_convert.ipynb
│   ├── Lab2_Chunking.ipynb
│   └── Lab3_RAG.ipynb
├── mkdocs.yml              # Configuración del sitio de documentación
├── pyproject.toml          # Dependencias del proyecto
└── uv.lock                 # Lockfile de dependencias
```

## Contribución y soporte

¿Encontraste un error o tienes una sugerencia? ¡Tu ayuda es bienvenida!

- 🐛 **Issues**: Abre un [Issue en GitHub](https://github.com/simonsanvil/docling-workshop-pycones-2025/issues) para reportar problemas o sugerir mejoras
- 🔀 **Pull Requests**: Envía un PR con tus mejoras (revisa [CONTRIBUTING.md](CONTRIBUTING.md) para más detalles)
- 💬 **Discusiones**: Únete a las [Discussions](https://github.com/simonsanvil/docling-workshop-pycones-2025/discussions) para preguntas generales

## Licencia

Este proyecto está licenciado bajo la [Licencia MIT](LICENSE).

Basado en el workshop original de [IBM Granite Community](https://github.com/ibm-granite-community/docling-workshop).