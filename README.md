<p align="center">
  <img src="img/git.png" alt="Logo" width="100"/>
</p>

# Git/GitHub | SCESI

<p align="center">
  <img src="img/img1.png" alt="Introducción a Git" width="400"/>
</p>

---

## Ramas en Git

### ¿Qué es una rama?

Una rama en Git es un apuntador móvil que marca una serie de commits. Representa una línea de desarrollo independiente y permite realizar cambios sin afectar el proyecto principal.

Por defecto, todos los repositorios comienzan en la rama main, pero se pueden crear múltiples ramas para nuevas funcionalidades, pruebas o correcciones.

### ¿Para qué sirven las ramas?

Las ramas son fundamentales para:

- Desarrollar nuevas funcionalidades sin modificar el código estable.
- Trabajar en equipo sin sobrescribir los cambios de otros.
- Realizar pruebas, correcciones y prototipos sin riesgo.
- Organizar mejor el flujo de trabajo y aislar tareas específicas.

Trabajar con ramas nos permite mantener un desarrollo no lineal, ordenado y fácilmenteble.

### Creación de una nueva rama

Para crear una nueva rama, podemos usar:

```bash
git branch nombre-de-la-rama
```

Para crear y moverse directamente a ella:

```bash
git checkout -b nombre-de-la-rama
```

Después de trabajar en una rama y hacer los commits necesarios, se puede volver a la rama principal (main) y fusionar los cambios.

