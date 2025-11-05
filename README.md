# Usar repositorios con git y github 

## CONFIGURACION

Para configurar **Git globalmente** con tu nombre de usuario y correo electrónico (los que se usarán en todos los repositorios de tu sistema), haz lo siguiente desde la terminal:

---

### 🧭 1. Configurar nombre de usuario

```bash
git config --global user.name "Tu Nombre"
```

Ejemplo:

```bash
git config --global user.name "ElJoho"
```

---

### ✉️ 2. Configurar correo electrónico

```bash
git config --global user.email "tucorreo@example.com"
```

Ejemplo:

```bash
git config --global user.email "johalopezari@unal.edu.co"
```

---

### 📋 3. Verificar la configuración

```bash
git config --global --list
```

Esto debería mostrar algo como:

```
user.name=El Joho
user.email=eljoho@gmail.com
```

---

### 💡 Tip adicional

Si quieres editar el archivo directamente:

```bash
nano ~/.gitconfig
```

Ahí verás algo como:

```ini
[user]
    name = El Joho
    email = eljoho@gmail.com
```

---

