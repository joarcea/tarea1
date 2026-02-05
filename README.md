# tarea1 - Aprender sobre Etiquetas (Git Tags)

Este repositorio es un ejemplo práctico para aprender sobre etiquetas de Git.

## ¿Qué son las etiquetas de Git?

Las etiquetas (tags) en Git son referencias que apuntan a puntos específicos en la historia de Git. Son útiles para marcar versiones de lanzamiento (v1.0, v2.0, etc.).

## Tipos de etiquetas

### 1. Etiquetas Ligeras (Lightweight Tags)
Las etiquetas ligeras son simplemente un puntero a un commit específico.

```bash
# Crear una etiqueta ligera
git tag v1.0

# Listar todas las etiquetas
git tag
```

### 2. Etiquetas Anotadas (Annotated Tags)
Las etiquetas anotadas son objetos completos en la base de datos de Git. Contienen información adicional como el nombre del creador, email, fecha y mensaje.

```bash
# Crear una etiqueta anotada
git tag -a v2.0 -m "Versión 2.0 - Segunda versión del proyecto"

# Ver información de una etiqueta
git show v2.0
```

## Comandos útiles

```bash
# Listar todas las etiquetas
git tag

# Ver detalles de una etiqueta específica
git show <nombre-etiqueta>

# Crear etiqueta ligera
git tag <nombre-etiqueta>

# Crear etiqueta anotada con mensaje
git tag -a <nombre-etiqueta> -m "mensaje"

# Etiquetar un commit específico
git tag -a <nombre-etiqueta> <commit-hash> -m "mensaje"

# Enviar etiquetas al repositorio remoto
git push origin <nombre-etiqueta>

# Enviar todas las etiquetas
git push origin --tags

# Eliminar una etiqueta local
git tag -d <nombre-etiqueta>

# Eliminar una etiqueta remota
git push origin --delete <nombre-etiqueta>
```

## Ejemplo práctico

Este repositorio incluye ejemplos de ambos tipos de etiquetas para demostrar su uso.
