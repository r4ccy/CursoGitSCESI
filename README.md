<p align="center">
  <img src="img/git.png" alt="Logo" width="100"/>
</p>

# Git/GitHub | SCESI

## Introducción a Git

---

Sistema de control de versiones para gestionar cambios en archivos, desde código hasta documentos. **Más que herramientas, es una filosofía de trabajo.**

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

### Breve historia de Git

| Año  | Hito                                                                 |
| ---- | -------------------------------------------------------------------- |
| 1986 | **CVS** (sistema centralizado y lento).                              |
| 2005 | **Git** creado por Linus Torvalds para Linux (rápido y distribuido). |
| 2008 | Nace **GitHub** (plataforma social para repositorios Git).           |
| 2018 | Microsoft compra GitHub (pero Git sigue siendo *open-source*).       |
| 2024 | Git domina el 90% del mercado (alternativas: Mercurial, SVN).        |

### ¿Qué es Git?

Git es como una máquina del tiempo para tus archivos. Permite guardar cada cambio importante, volver a versiones anteriores y colaborar sin conflictos ni pérdida de información.

### ¿Qué es un repositorio?

En Git, un repositorio es el corazón del proyecto: contiene los archivos y todo su historial. Puede ser:

- **Local:** Almacenado en la máquina del usuario.
- **Remoto:** Alojado en plataformas como GitHub o GitLab para facilitar la colaboración.

Cuando usamos `git init`, convertimos una carpeta común en un repositorio local.

<p align="center">
  <img src="img/repositorio.png" alt="Repositorio local vs remoto" width="280"/><br>
  <em>Figura: Relación entre repositorio local y remoto en Git.</em>
</p>

