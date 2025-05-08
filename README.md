<p align="center">
  <img src="img/git.png" alt="Logo" width="100"/>
</p>

# Git/GitHub | SCESI

## HEAD
---

En Git, HEAD es un puntero que siempre apunta al commit actual dentro de la rama activa. Es el marcador que indica dónde estás parado en el historial de versiones, literalmente te dice "estás aquí".

Cuando hacemos un nuevo commit, HEAD avanza al commit más reciente. Si cambiamos de rama o hacemos checkout a un commit anterior, HEAD también se actualiza para reflejar ese movimiento.

<p align="center">
  <img src="img/githead.webp" alt="HEAD apuntando a master en Git" width="500"/>
  <br>
  <em>Figura 1: HEAD apunta a la rama actual (master), la cual a su vez apunta al último commit.</em>
</p>

### Importancia del HEAD

- Permite identificar el estado actual del repositorio.
- Facilita la navegación entre ramas y versiones.
- Es clave para entender operaciones como checkout, reset y rebase.

Podemos imaginar al HEAD como un mensaje que nos dice "Estás aquí" en un mapa de commits. Siempre apunta al último commit visible en la rama donde se esta trabajando.

### Situaciones típicas con HEAD

1. **HEAD en una rama activa:**

```bash
HEAD -> main
```

2. **HEAD en estado detached (desvinculado)**

Cuando hacemos checkout a un commit específico (no una rama), HEAD entra en estado "detached". Esto significa que no está asociado a una rama. Si hacemos un commit desde allí, no se vinculará a ninguna rama existente. Por ejemplo:

```bash
git checkout 3f2a1e7
```

Resultado:

```bash
HEAD detached at 3f2a1e7
```

<p align="center">
  <img src="img/headtype.png" alt="HEAD Attached vs Detached en Git" width="600"/>
  <br>
  <em>Figura 2: Comparación entre HEAD adjunto a una rama y HEAD separado apuntando directamente a un commit.</em>
</p>
