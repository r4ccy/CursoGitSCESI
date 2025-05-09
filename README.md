<p align="center">
  <img src="img/git.png" alt="Logo" width="100"/>
</p>

# Curso de Git/GitHub | SCESI

## Deshacer cambios en Git

---

### ¿En qué casos deshacemos cambios?

Hacemos cambios cuando:

- El proyecto dejó de funcionar correctamente.
- Se quiere recuperar una parte del código eliminado.
- Queremos restaurar archivos borrados por error.

## Comandos destructivos y no destructivos

Git cuenta herramientas para revertir cambios según su nivel de impacto:

- **Comandos destructivos:** Afectan directamente el historial de commits.
- **Comandos no destructivos:** Revierten cambios sin modificar el historial.

## Comandos para deshacer cambios

### git reset

Nos permite deshacer commits y mover el puntero de HEAD. Tenemos dos caminos que podemos considerar.:

- **--soft**: Elimina el commit, pero mantiene los cambios en el área de staging.
- **--hard**: Elimina el commit y también los cambios del área de trabajo.

```bash
git reset --soft HEAD~1
git reset --hard HEAD~1
git reset --soft <hash>
git reset --hard <hash>
```

```
git reset --soft HEAD~1 : Elimina el último commit pero mantiene 
los cambios en staging, listos para commitear de nuevo.

git reset --hard HEAD~1 : Elimina el último commit y también borra 
los cambios del área de trabajo.

git reset --soft <hash> : Revierte el historial hasta un commit
 específico y conserva todos los cambios desde entonces en staging.

git reset --hard <hash> : Vuelve el proyecto al estado exacto de un
 commit anterior, eliminando todos los cambios posteriores.
```

### git reverse

Lo que hace es revertir un commit específico sin modificar el historial. Crea un nuevo commit con el efecto inverso.

```bash
git revert HEAD~1
git revert <hash>
```

```
git revert HEAD~1 : Revierte el commit anterior al actual, creando 
un nuevo commit que deshace sus cambios, sin borrar historial.

git revert <hash> :Revierte un commit específico identificado por
 su hash, también sin eliminarlo, solo deshaciendo sus efectos.
```

Es ideal si ya se hizo push al repositorio y no deseamos reescribir el historial compartido.
