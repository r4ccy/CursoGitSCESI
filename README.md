<p align="center">
  <img src="img/git.png" alt="Logo" width="100"/>
</p>

# Curso Git/GitHub | SCESI

Este repositorio documenta el contenido aprendido en el curso de control de versiones con Git y GitHub, impartido por SCESI. Cada clase se desarrolla en una rama independiente, con apuntes organizados, prácticas y comandos aplicados en diferentes ramas.

<p align="center">
  <img src="img/img1.png" alt="Introducción a Git" width="400"/>
</p>

---

## Clase 1 – Introducción a Git

En la primera clase se abordó el concepto de control de versiones y la razón de por qué se ha vuelto una herramienta esencial en el desarrollo de software.

### ¿Qué es un sistema de control de versiones?

Es un sistema que permite registrar y organizar los cambios realizados en los archivos de un proyecto a lo largo del tiempo. Permite ver el historial de cambios, identificar quién hizo cada modificación y cuándo, así como volver atrás en caso de errores. Además, facilita el trabajo en equipo sin que los cambios de una persona interfieran con los de otra.

<p align="center">
  <img src="img/versiones.png" alt="Historial de versiones en Git" width="500"/><br>
  <em>Figura: Representación visual del historial de versiones en Git, donde cada punto corresponde a un commit con cambios progresivos en un archivo.</em>
</p>

### Importancia de un control de versiones

- **Rendimiento:** Git guarda solo lo que cambia, no todo el archivo.
- **Seguridad:** Permite rastrear cada cambio y quién lo realizó.
- **Flexibilidad:** Posibilita trabajar en paralelo mediante ramas, sin seguir un flujo lineal.

### ¿Qué es Git?

Git es como una máquina del tiempo para tus archivos. Permite guardar cada cambio importante, volver a versiones anteriores y colaborar sin conflictos ni pérdida de información.

### ¿Qué es un repositorio?

En Git, un repositorio es el corazón del proyecto: contiene los archivos y todo su historial. Puede ser:

- **Local:** Almacenado en la máquina del usuario.
- **Remoto:** Alojado en plataformas como GitHub o GitLab para facilitar la colaboración.

Cuando usamos git init, convertimos una carpeta común en un repositorio local.

<p align="center">
  <img src="img/repositorio.png" alt="Repositorio local vs remoto" width="280"/><br>
  <em>Figura: Relación entre repositorio local y remoto en Git.</em>
</p>



## Clase 2 – Estados, Commits y creación de ramas

### Estados en Git
Git gestiona los archivos mediante tres estados que reflejan su situación en el flujo de trabajo:

- **Modified (Modificado):** el archivo fue editado pero aún no está listo para ser guardado.
- **Staged (Preparado):** el archivo fue marcado con `git add` y está listo para el siguiente commit.
- **Committed (Confirmado):** el archivo ya forma parte del historial del repositorio.

Comprender estos estados permite dominar el flujo de trabajo: modificar → preparar → confirmar.

### ¿Qué es un commit?
Un commit es una instantánea del estado del proyecto. Cada commit almacena:
- Archivos preparados (staged).
- Información del autor.
- Fecha y hora del cambio.
- Un mensaje que describe el propósito del commit.

> Ejemplos de buenos mensajes:
> - `Agregar sección sobre ramas`
> - `Corregir error en ejemplo de commit`

Evitar mensajes genéricos como “cambios” o “update”.

### HEAD en Git
El `HEAD` es un puntero que indica el commit actual en la rama activa. Al hacer nuevos commits o cambiar de rama, `HEAD` se actualiza.

- En la rama `main`, `HEAD` apunta al último commit de `main`.
- Si se cambia de rama, `HEAD` apunta al último commit de la nueva rama.

<p align="center">
  <img src="img/Head.jpeg" alt="HEAD y ramas en Git" width="400"/>
  <br>
  <em>Figura: HEAD como puntero actual en la estructura de ramas en Git.</em>
</p>

### Introducción a ramas
Una rama representa una línea de desarrollo independiente.

Beneficios:
- Facilita el trabajo paralelo.
- Permite probar ideas sin afectar el código principal.
- Mejora la organización del proyecto.

La rama por defecto es `main`, donde suele mantenerse el código estable.

### Comandos útiles para ramas
Crear una nueva rama sin cambiarse a ella:
```bash
git branch nombre-de-la-rama
