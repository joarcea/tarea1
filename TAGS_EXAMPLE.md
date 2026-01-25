# Ejemplos de Etiquetas en este Repositorio

Este archivo documenta las etiquetas creadas en este repositorio como parte del aprendizaje sobre Git tags.

## Etiquetas Creadas

### v1.0-lightweight
- **Tipo**: Etiqueta Ligera (Lightweight Tag)
- **Descripción**: Esta es una etiqueta ligera que simplemente apunta a un commit específico sin metadata adicional.
- **Uso**: Las etiquetas ligeras son útiles para marcar puntos rápidamente sin necesidad de información adicional.

Para ver esta etiqueta:
```bash
git show v1.0-lightweight
```

### v1.0-annotated
- **Tipo**: Etiqueta Anotada (Annotated Tag)
- **Descripción**: Esta es una etiqueta anotada con metadata completa incluyendo autor, fecha y mensaje.
- **Mensaje**: "Primera versión anotada - Ejemplo de etiqueta anotada con metadata completa"
- **Uso**: Las etiquetas anotadas son recomendadas para versiones de lanzamiento porque almacenan información completa.

Para ver esta etiqueta con todos sus detalles:
```bash
git show v1.0-annotated
```

## Verificar las Etiquetas

Puedes listar todas las etiquetas en este repositorio con:
```bash
git tag
```

O listar con más detalles:
```bash
git tag -n
```

## Diferencias entre los Tipos de Etiquetas

| Característica | Ligera | Anotada |
|----------------|--------|---------|
| Almacena metadata | No | Sí |
| Tiene autor | No | Sí |
| Tiene fecha | No | Sí |
| Tiene mensaje | No | Sí |
| Es un objeto Git | No | Sí |
| Recomendada para releases | No | Sí |
| Más rápida de crear | Sí | No |

## Nota sobre Tags Remotos

Las etiquetas creadas localmente deben ser enviadas explícitamente al repositorio remoto:
```bash
# Enviar una etiqueta específica
git push origin v1.0-annotated

# Enviar todas las etiquetas
git push origin --tags
```
