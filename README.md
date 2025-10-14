# PyConES 2025 | Docling Workshop

Repositorio de la workshop de Docling presentado en la [PyConES 2025](https://2025.es.pycon.org/). Aquí encontrarás el material de la workshop, la documentación y los notebooks prácticos usados durante la sesión.

- Sitio de la documentación: https://simonsanvil.github.io/docling-workshop-pycones-2025/
- Proyecto Docling: https://docling-project.github.io/docling/

## ¿Qué vas a aprender?

Al finalizar esta workshop serás capaz de:
- Convertir documentos complejos a formatos útiles para IA preservando su estructura con Docling.
- Entender y aplicar técnicas de chunking y vectorización para mejorar tu sistema de recuperación de información.
- Construir un sistema RAG multimodal transparente y verificable.

## Contenidos de la workshop

La documentación completa de la workshop está en [docs/](/docs/) y publicada en el sitio anterior. Recomendamos seguir la navegación del sitio web publicado para una mejor experiencia.

La documentación se divide en las siguientes secciones:

- [Introducción](/docs/README.md): Una pequeña introducción a Docling y contenido de la workshop.
- [Preparación de entorno](/docs/pre-work/README.md): Instrucciones para preparar tu entorno de trabajo y ejecutar los notebooks.

Los tres notebooks prácticos donde se desarrolla la parte práctica de la workshop:

- [`Lab 1 – Conversión de documentos`](/docs/lab-1/README.md) [![Conversión de documentos con Docling - Notebook](https://colab.research.google.com/assets/colab-badge.svg "Abrir en Colab")](https://colab.research.google.com/github/simonsanvil/docling-workshop-pycones-2025/blob/703a299b236366e05f79f5df19b414ed03721de7/notebooks/Lab1_Docling_convert.ipynb)
- [`Lab 2 – Chunking y vectorización`](/docs/lab-2/README.md) [![Chunking y vectorización con Docling - Notebook](https://colab.research.google.com/assets/colab-badge.svg "Abrir en Colab")](https://colab.research.google.com/github/simonsanvil/docling-workshop-pycones-2025/blob/703a299b236366e05f79f5df19b414ed03721de7/notebooks/Lab2_Hybrid_Chunking.ipynb)
- [`Lab 3 – RAG multimodal`](/docs/lab-3/README.md) [![RAG multimodal con Docling - Notebook](https://colab.research.google.com/assets/colab-badge.svg "Abrir en Colab")](https://colab.research.google.com/github/simonsanvil/docling-workshop-pycones-2025/blob/703a299b236366e05f79f5df19b414ed03721de7/notebooks/Lab3_RAG.ipynb)

Puedes abrirlos en local (ver sección de preparación) o ejecutarlos en Google Colab pulsando en los botones correspondientes.

## Requisitos previos

- Git y Python 3.10, 3.11 o 3.12
- Cuenta en [Replicate](https://replicate.com/) para usar modelos de IA en la nube.
- Para ejecutar notebooks en local: Jupyter Notebook o JupyterLab

Consulta detalles y pasos en: [docs/pre-work/README.md](/docs/pre-work/README.md) (Preparación).

## Preparación rápida

Si trabajas con `uv` (`pip install uv`), puedes instalar dependencias con:

```bash
# instalar solo dependencias de los notebooks (necesario para ejecutar los labs)
uv sync --no-dev
```

Si además quieres servir la documentación localmente para verla en tu navegador:

```bash
# Instalar dependencias del proyecto (incluye grupo dev)
uv sync --all-groups

# Servir la documentación localmente
uv run mkdocs serve
```

Para preparación detallada (entornos, Jupyter, variables de entorno para Replicate, etc.), sigue los pasos en [docs/pre-work/README.md](/docs/pre-work/README.md).

## Construir la documentación

Para generar el sitio estático en `site/`:

```bash
uv run mkdocs build --clean
```

La documentación utiliza [MkDocs Material](https://squidfunk.github.io/mkdocs-material/) con algunas personalizaciones. El tema y configuración están en `mkdocs.yml`.

## Estructura del repositorio

- `docs/` – Fuente de la documentación (MkDocs)
  - `images/` – Imágenes usadas en la documentación
  - `css/custom.css` – Estilos personalizados.
  - `pre-work/`, `lab-1/`, `lab-2/`, `lab-3/` – Páginas de los labs
- `notebooks/` – Notebooks de los laboratorios
<!-- - `materials/` – Material de apoyo (si aplica) -->
<!-- - `output/` – Artefactos generados (p.ej. conversiones con Docling) -->
<!-- - `site/` – Salida estática generada por MkDocs (no editar a mano) -->
- `mkdocs.yml` – Configuración del sitio de documentación
- `pyproject.toml` / `uv.lock` – Dependencias y bloqueo de versiones

## Contribución y soporte

- ¿Sugerencias, dudas o problemas? Abre un "Issue" en GitHub.
- Pull Requests bienvenidas para mejoras en documentación, ejemplos o correcciones.

## Créditos

- [IBM Granite Community](https://github.com/ibm-granite-community)
- Autoría de contenidos y contribuciones: ver la sección de Créditos dentro de la documentación.