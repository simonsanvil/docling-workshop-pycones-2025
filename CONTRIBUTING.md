# Guía de Contribución

¡Gracias por tu interés en contribuir al Docling Workshop de PyConES 2025! 🎉

Este documento proporciona pautas y mejores prácticas para contribuir al proyecto.

## 🚀 Cómo Contribuir

### Reportar Problemas

Si encuentras un error o tienes una sugerencia:

1. Verifica que el problema no haya sido reportado previamente en [Issues](https://github.com/simonsanvil/docling-workshop-pycones-2025/issues)
2. Abre un nuevo Issue con:
   - Un título descriptivo
   - Descripción clara del problema o sugerencia
   - Pasos para reproducir (si es un error)
   - Capturas de pantalla si aplica
   - Información del entorno (SO, versión de Python, etc.)

### Proponer Cambios

Para contribuir con código o documentación:

1. **Fork el repositorio**
   ```bash
   # Haz fork del proyecto en GitHub y clona tu fork
   git clone https://github.com/TU-USUARIO/docling-workshop-pycones-2025.git
   cd docling-workshop-pycones-2025
   ```

2. **Crea una rama para tu contribución**
   ```bash
   git checkout -b feature/descripcion-corta
   # o
   git checkout -b fix/descripcion-del-fix
   ```

3. **Configura tu entorno de desarrollo**
   ```bash
   # Instala uv si no lo tienes
   pip install uv
   
   # Instala todas las dependencias (incluyendo dev)
   uv sync --all-groups
   ```

4. **Haz tus cambios**
   - Escribe código claro y documentado
   - Sigue las convenciones existentes en el proyecto
   - Actualiza la documentación si es necesario
   - Asegúrate de que los notebooks ejecutan correctamente

5. **Prueba tus cambios**
   ```bash
   # Si modificaste la documentación, construye y visualiza localmente
   uv run mkdocs serve
   
   # Si modificaste notebooks, ejecútalos para verificar que funcionan
   jupyter notebook notebooks/TU_NOTEBOOK.ipynb
   ```

6. **Commit y Push**
   ```bash
   git add .
   git commit -m "tipo: descripción concisa del cambio"
   git push origin feature/descripcion-corta
   ```

7. **Abre un Pull Request**
   - Ve a tu fork en GitHub
   - Haz clic en "New Pull Request"
   - Describe claramente qué cambios hiciste y por qué
   - Menciona cualquier Issue relacionado con `Fixes #numero-issue`

## 📝 Estándares de Contribución

### Mensajes de Commit

Usa mensajes de commit descriptivos siguiendo el formato:

```
tipo: descripción concisa

Descripción más detallada si es necesario.

Refs #issue-number
```

Tipos comunes:
- `docs:` - Cambios en documentación
- `feat:` - Nueva funcionalidad
- `fix:` - Corrección de errores
- `style:` - Cambios de formato sin afectar funcionalidad
- `refactor:` - Refactorización de código
- `test:` - Adición o modificación de tests
- `chore:` - Mantenimiento general

### Documentación

- Escribe en español claro y conciso
- Usa Markdown para formatear
- Incluye ejemplos de código cuando sea posible
- Añade imágenes o diagramas para explicaciones complejas

### Notebooks

- Incluye comentarios explicativos en español
- Asegúrate de que todas las celdas ejecutan sin errores
- Limpia las salidas antes de hacer commit (opcional pero recomendado)
- Mantén un orden lógico en las celdas

### Código Python

- Sigue [PEP 8](https://pep8.org/) para estilo de código
- Usa nombres de variables descriptivos en inglés o español
- Añade docstrings para funciones y clases
- Mantén las funciones pequeñas y enfocadas

## 🔍 Revisión de Pull Requests

Los maintainers revisarán tu PR y podrán:
- Aprobar y fusionar directamente
- Solicitar cambios o aclaraciones
- Sugerir mejoras

Por favor, sé paciente y responde a los comentarios de revisión.

## 💡 Ideas para Contribuir

¿No sabes por dónde empezar? Aquí hay algunas ideas:

- Mejorar la claridad de las instrucciones de instalación
- Añadir más ejemplos en los notebooks
- Corregir errores tipográficos o gramaticales
- Mejorar el diseño o estilo de la documentación
- Añadir secciones de troubleshooting
- Traducir documentación adicional
- Optimizar código en los notebooks
- Añadir tests o validaciones

## 📞 Contacto

Si tienes preguntas sobre cómo contribuir:
- Abre una [Discussion](https://github.com/simonsanvil/docling-workshop-pycones-2025/discussions)
- Contacta a los maintainers en los Issues

## 🙏 Reconocimientos

Todos los contribuidores serán reconocidos en la documentación del proyecto.

¡Gracias por hacer de este workshop un mejor recurso para la comunidad! 🐍✨
