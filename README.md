# PyConES 2025 | Docling Workshop

Repositorio de la workshop de Docling presentado en la [PyConES 2025](https://2025.es.pycon.org/). Aquí encontrarás el material de la workshop, la documentación y los notebooks prácticos usados durante la sesión.

- Sitio de la documentación: https://ibm-granite-community.github.io/docling-workshop
- Proyecto Docling: https://docling-project.github.io/docling/

## ¿Qué vas a aprender?

Al finalizar esta workshop serás capaz de:
- Convertir documentos complejos a formatos útiles para IA preservando su estructura con Docling.
- Entender y aplicar técnicas de chunking y vectorización para mejorar tu sistema de recuperación de información.
- Construir un sistema RAG multimodal transparente y verificable.

## Contenidos de la workshop

La documentación completa de la workshop está en [docs/](/docs/) y publicada en el sitio anterior. Puntos de entrada rápidos:

- Introducción: [`docs/README.md`](/docs/README.md)
- Preparación (Lab 0): [`docs/pre-work/README.md`](/docs/pre-work/README.md)
- Lab 1 – Conversión de documentos: [`docs/lab-1/README.md`](/docs/lab-1/README.md)
- Lab 2 – Chunking y vectorización: [`docs/lab-2/README.md`](/docs/lab-2/README.md)
- Lab 3 – RAG multimodal: [`docs/lab-3/README.md`](/docs/lab-3/README.md)

Recomendamos seguir la navegación del sitio web publicado para una mejor experiencia.

## Requisitos previos

- Git y Python 3.10, 3.11 o 3.12
- (Opcional, para algunas opciones del Lab 3) Cuenta en Replicate y token de API
- Para ejecutar notebooks en local: Jupyter Notebook o JupyterLab

Consulta detalles y pasos en: [docs/pre-work/README.md](/docs/pre-work/README.md) (Preparación).

## Notebooks

Los notebooks de la workshop se encuentran en `notebooks/`:
- [`Lab1_Docling_convert.ipynb`](/notebooks/Lab1_Docling_convert.ipynb)
- [`Lab2_Hybrid_Chunking.ipynb`](/notebooks/Lab2_Hybrid_Chunking.ipynb)
- [`Lab3_RAG.ipynb`](/notebooks/Lab3_RAG.ipynb) (con Replicate)
- [`LabX_Agents.ipynb`](/notebooks/LabX_Agents.ipynb) (material adicional)

Puedes abrirlos en local (ver sección de preparación) o ejecutarlos en Google Colab. En la documentación de cada lab encontrarás los badges/enlaces directos a GitHub y Colab.

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