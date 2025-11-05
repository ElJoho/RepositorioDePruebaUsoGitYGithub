
## Ver el historial de commits


### 🔙 Volver a un commit pasado

1. Mira los commits:

   ```bash
   git log --oneline
   ```
2. Copia el ID (por ejemplo `e5f6g7h`)
3. Vuelve a ese commit:

   ```bash
   git checkout e5f6g7h
   ```

---

### 🔁 Volver del commit pasado al último cambio

Para regresar al estado más reciente:

```bash
git checkout main
```
---

💡 *Eso es todo.*
(`checkout` para ir a un commit pasado, y `checkout main` para volver al último).


## 🧩 Resumen rápido

| Acción                       | Comando                   | Qué hace                    |
| ---------------------------- | ------------------------- | --------------------------- |
| Ver historial                | `git log --oneline`       | Lista de commits            |
| Ir a un commit pasado        | `git checkout <hash>`     | Explora el pasado           |
| Volver al último estado      | `git checkout main`       | Regresa a la rama actual    |
| Revertir commit (sin borrar) | `git revert <hash>`       | Crea un commit inverso      |
| Reset suave                  | `git reset --soft <hash>` | Vuelve manteniendo staging  |
| Reset duro                   | `git reset --hard <hash>` | Elimina cambios posteriores |
| Recuperar commits borrados   | `git reflog`              | Muestra historial de HEAD   |
