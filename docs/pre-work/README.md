---
title: Preparación
description: Preparación
logo: images/DoclingDuck.png
---

# Preparación

Los laboratorios de la workshop son [notebooks de Jupyter](https://jupyter.org/). Los notebooks pueden ejecutarse:
 <!-- en tu ordenador o de forma remota en el servicio [Google Colab](https://colab.research.google.com). 

## Ejecución de notebooks -->

<!-- Los notebooks pueden ejecutarse: -->

- [Localmente en tu equipo](#ejecucion-de-notebooks-localmente) (para el cual necesitarás instalar algunas dependencias) O
- [De forma remota en Google Colab](#ejecucion-de-notebooks-de-forma-remota-colab)

Sigue las instrucciones en una de las siguientes secciones según cómo prefieras ejecutarlos.

## Ejecución de notebooks localmente

Si quieres ejecutar los notebooks de los laboratorios localmente en tu ordenador, se recomienda contar con:

- Un ordenador o portátil: mínimo 8 GB de RAM (16 GB recomendado)
- Conocimientos de [Git](https://git-scm.com/) y [Python](https://www.python.org/): Lo suficiente para instalar dependencias y ejecutar Jupyter Notebooks
- (Opcional) Un IDE como [VS Code](https://code.visualstudio.com/) o [PyCharm](https://www.jetbrains.com/pycharm/) para editar y ejecutar los notebooks comodamente.

Si alguna de estas no es el caso, te recomendamos ir a la sección [Ejecución de notebooks de forma remota (Colab)](#ejecucion-de-notebooks-de-forma-remota-colab).

Para ejecutar los notebooks de los laboratorios localmente en tu equipo, sigue estos pasos:

- [Prerrequisitos locales](#prerrequisitos-locales)
- [Clonar el repositorio de la workshop](#clonar-el-repositorio-de-la-workshop-de-docling)
- [Instalar Jupyter](#instalar-jupyter)

### Prerrequisitos locales

- Git
- Python 3.10, 3.11 o 3.12

### Clonar el repositorio de la workshop de Docling

Clona el repositorio de la workshop y entra en el directorio del repositorio.

```shell
git clone https://github.com/IBM/docling-workshop.git
cd docling-workshop
```


### Instalar Jupyter

!!! note "Usa un entorno virtual"
    Antes de instalar dependencias y para evitar conflictos en tu entorno, es aconsejable utilizar un [entorno virtual (venv)](https://docs.python.org/3/library/venv.html).

1. Crea un entorno virtual:

    ```shell
    python3 -m venv --upgrade-deps --clear venv
    ```

2. Activa el entorno virtual ejecutando:

    ```shell
    source venv/bin/activate
    ```

3. Instala Jupyter Notebook en el entorno virtual:

    ```shell
    python3 -m pip install --require-virtualenv notebook ipywidgets
    ```

    Para más información, consulta las [instrucciones de instalación de Jupyter](https://jupyter.org/install).

4. Para abrir un notebook en Jupyter (con el entorno virtual activo), ejecuta:

    ```shell
    jupyter notebook <notebook-file-path>
    ```

    Alternativamente, si tienes instalado VS Code, puedes habilitar la extensión de Jupyter Notebooks para VS Code (instrucciones [aquí](https://code.visualstudio.com/docs/datascience/jupyter-notebooks)) y abrir los notebooks directamente en VS Code.

### Uso de los modelos de Granite con Replicate

En el laboratorio 3 utilizaras modelos de IA generativa [Granite](https://www.ibm.com/granite) para construir un sistema RAG multimodal. Para ello usaremos [Replicate](https://replicate.com/), una plataforma en la nube que aloja y sirve modelos de IA por ti.

#### Instrucciones para configurar Replicate

1. Crea una cuenta en [Replicate](https://replicate.com/). Necesitarás una cuenta de [GitHub](https://github.com/) para hacerlo.

2. Añade saldo a tu cuenta de Replicate (opcional). Para facilitar probar los modelos en Replicate, utiliza [este enlace](https://replicate.com/invites/a8717bfe-2f3d-4a52-88ed-1356231cdf03) para añadir una pequeña cantidad de crédito a tu cuenta cortesía de [la(https://github.com/ibm-granite-community) comunidad de IBM Granite].

3. Crea un [token de API](https://replicate.com/account/api-tokens) de Replicate.

4. Establece tu token de API de Replicate como una variable de entorno en la terminal donde vayas a ejecutar el notebook:

    ```shell
    export REPLICATE_API_TOKEN=<your_replicate_api_token>
    ```

## Ejecución de notebooks de forma remota (Colab)

Para ejecutar los notebooks de los laboratorios de forma remota usando [Google Colab](https://colab.research.google.com), sigue estos pasos:

- [Prerrequisitos de Colab](#prerrequisitos-de-colab)
- [Servir los modelos de Granite con Replicate](#servir-los-modelos-de-granite-con-replicate)

!!! note "Velocidad de ejecución de notebooks en Colab" 
    En Colab, el runtime por defecto usa **CPUs**. Considera cambiar el tipo de entorno en Colab para aumentar la velocidad de ejecución, especialmente si tienes otras limitaciones como una conexión lenta. En la barra de navegación, selecciona `Runtime->Change runtime type` y elige aceleración por **GPU o TPU**.

### Prerrequisitos de Colab

- [Google Colab](https://colab.research.google.com) requiere una cuenta de Google con la que hayas iniciado sesión.

### Servir los modelos de Granite con Replicate

En el laboratorio 3 utilizaras modelos de IA generativa [Granite](https://www.ibm.com/granite) para construir un sistema RAG multimodal. Para ello usaremos [Replicate](https://replicate.com/), una plataforma en la nube que aloja y sirve modelos de IA por ti.

#### Instrucciones para configurar Replicate

1. Crea una cuenta en [Replicate](https://replicate.com/). Necesitarás una cuenta de [GitHub](https://github.com/).

2. Añade saldo a tu cuenta de Replicate (opcional). Para facilitar probar los modelos Granite en Replicate, utiliza [este enlace](https://replicate.com/invites/a8717bfe-2f3d-4a52-88ed-1356231cdf03) para añadir una pequeña cantidad de crédito a tu cuenta cortesía de [la comunidad de IBM Granite](https://github.com/ibm-granite-community).

3. Crea un [API token](https://replicate.com/account/api-tokens) de Replicate.

4. Añade tu token de API de Replicate al gestor de secretos de Colab para guardarlo de forma segura. Abre [Google Colab](https://colab.research.google.com) y haz clic en la pestaña `🔑 Secrets` del panel izquierdo. Pulsa "New Secret" e introduce `REPLICATE_API_TOKEN` como clave; pega tu token en el campo de valor. Activa el botón de la izquierda para permitir que el notebook acceda al secreto.
