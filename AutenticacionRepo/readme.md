
### 1. Clonar un repositorio remoto

Si el repositorio está en GitHub, copia su URL (por ejemplo:
`https://github.com/ElJoho/RepositorioDePruebaUsoGitYGithub.git`)

Luego en la terminal:

```bash
git clone https://github.com/ElJoho/RepositorioDePruebaUsoGitYGithub.git
```

Esto creará una carpeta llamada **mi_proyecto** con todo el contenido del repo.
Entra a ella:

```bash
cd mi_proyecto
```

---

### 🔍 2. Ver el estado del repositorio

Muestra qué archivos han cambiado o están sin guardar:

```bash
git status
```

Ejemplo de salida:

```
En la rama main
Cambios no preparados para el commit:
  modificado: archivo.txt
Archivos sin seguimiento:
  nuevo_archivo.txt
```

---

### ➕ 3. Añadir archivos al área de preparación (staging)

Para agregar un archivo específico:

```bash
git add nombre_del_archivo
```

Para agregar **todos los archivos modificados o nuevos**:

```bash
git add .
```

---

### 💬 4. Crear un commit con descripción

Guarda los cambios en la historia local:

```bash
git commit -m "Descripción breve de los cambios"
```

Ejemplo:

```bash
git commit -m "Agrego función de control de motores"
```

---

### 🔐 5. Conectar al repositorio remoto usando un **token personal**

GitHub ya no permite autenticarse con contraseña desde la terminal.
Debes usar un **token (PAT)** que generas en
👉 [https://github.com/settings/tokens](https://github.com/settings/tokens)

Cuando clones o empujes (push), puedes usar dos formas:

### **Opción A – Clonar directamente con el token**

```bash
git clone https://<TOKEN>@github.com/nombre_usuario/nombre_repositorio
```

Ejemplo:

```bash
git clone https://ghp_token@github.com/ElJoho/mi_proyecto.git
```

*(No compartas tu token, funciona como una contraseña).*

### **Opción B – Actualizar la URL remota existente**

Si ya clonaste el repo sin el token, puedes actualizar la URL con:

```bash
git remote set-url origin https://<TOKEN>@github.com/nombre_usuario/nombre_repositorio
```

Ejemplo:

```bash
git remote set-url origin https://token@github.com/ElJoho/RepositorioDePruebaUsoGitYGithub
```

---

### 🚀 6. Subir tus cambios a GitHub

Finalmente, para enviar tus commits locales al repositorio remoto:

```bash
git push origin main
```

💡 *Si tu rama principal se llama `master`, usa `master` en lugar de `main`.*

---

### 🧩 Resumen rápido de comandos

| Acción                       | Comando                                                               |
| ---------------------------- | --------------------------------------------------------------------- |
| Clonar repo                  | `git clone URL`                                                       |
| Ver estado                   | `git status`                                                          |
| Agregar cambios              | `git add .`                                                           |
| Guardar cambios              | `git commit -m "mensaje"`                                             |
| Ver remoto actual            | `git remote -v`                                                       |
| Cambiar URL remota con token | `git remote set-url origin https://TOKEN@github.com/usuario/repo.git` |
| Subir cambios                | `git push origin main`                                                |

