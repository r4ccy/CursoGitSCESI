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

