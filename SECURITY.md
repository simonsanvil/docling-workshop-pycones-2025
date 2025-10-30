# Política de Seguridad

## Versiones Soportadas

Este proyecto es un repositorio educativo para un workshop. Actualmente mantenemos:

| Versión | Soportada          |
| ------- | ------------------ |
| main    | :white_check_mark: |

## Reportar una Vulnerabilidad

La seguridad de nuestros usuarios es una prioridad. Si descubres una vulnerabilidad de seguridad, por favor sigue estos pasos:

### Para Vulnerabilidades Críticas

Si encuentras una vulnerabilidad crítica que podría afectar a los usuarios del workshop:

1. **NO abras un Issue público**
2. Envía un correo a los mantenedores del proyecto describiendo:
   - Tipo de vulnerabilidad
   - Pasos para reproducir
   - Impacto potencial
   - Si es posible, una solución sugerida

### Para Problemas de Seguridad Menores

Para problemas de seguridad no críticos:

1. Abre un [Issue en GitHub](https://github.com/simonsanvil/docling-workshop-pycones-2025/issues/new)
2. Marca el issue con la etiqueta "security"
3. Describe el problema y su impacto

## Qué Esperamos

- Usa este proceso para reportar vulnerabilidades de forma responsable
- Dale tiempo razonable al equipo para responder antes de divulgar públicamente
- No explotar la vulnerabilidad para fines malintencionados

## Qué Puedes Esperar de Nosotros

- Responderemos a tu reporte lo antes posible
- Te mantendremos informado sobre el progreso de la resolución
- Te acreditaremos en las notas de la versión si lo deseas (a menos que prefieras permanecer anónimo)

## Dependencias

Este proyecto usa varias dependencias de terceros. Si encuentras vulnerabilidades en las dependencias:

1. Verifica si hay versiones actualizadas disponibles
2. Abre un Pull Request actualizando `pyproject.toml` y `uv.lock`
3. Documenta la vulnerabilidad y la solución en el PR

## Buenas Prácticas de Seguridad

Como usuario de este workshop, recomendamos:

- ✅ Nunca compartir tus API keys o tokens
- ✅ Usar variables de entorno para credenciales
- ✅ No subir notebooks con datos sensibles o credenciales
- ✅ Mantener tus dependencias actualizadas
- ✅ Usar entornos virtuales aislados

## Recursos de Seguridad

- [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- [Python Security Best Practices](https://python.readthedocs.io/en/latest/library/security_warnings.html)
- [GitHub Security Advisories](https://github.com/advisories)

Gracias por ayudar a mantener este proyecto seguro para todos. 🔒
