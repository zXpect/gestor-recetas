# 📄 Documentación del Proyecto 

Este documento registra el flujo de trabajo realizado con *Git y GitHub*, incluyendo ramas creadas, comandos ejecutados, PRs, merges y resolución de conflictos.

---

## 🔹 1. Ramas creadas y responsables

- *main* → Rama principal del repositorio. Responsable: Administrador del repo [Fabian(zXpect)]  
- *feature/recetas-italianas* → Recetas de Italia. Responsable: [Fabian(zXpect)]  
- *feature/recetas-colombianas* → Recetas de Colombia. Responsable: [Breider(Car0nte092)]  
- *feature/recetas-mexicanas* → Recetas de México. Responsable: [Breider(Car0nte092)]  

---

## 🔹 2. Comandos ejecutados

### 📌 Creación y cambio de ramas
```bash
git checkout -b feature/recetas-italianas
```

![Checkout branch](gestor-recetas/docs/img/checkout.png)

---

### 📌 Agregar y confirmar cambios
```bash
git add recetas/italianas.md
git add gestor-recetas/recetas/italianas.md
git commit -m "Agrego recetas italianas: Carbonara, Margherita y Parmigiana"
git commit -m "Corrijo formato en recetas italianas (títulos y separadores)"
git commit -m "Agrego notas y recomendaciones adicionales en recetas italianas"
```

---

### 📌 Verificar estado y commits
```bash
git status
git log
```

---

### 📌 Configuración de usuario
```bash
git config --global user.name "username"
```

---

### 📌 Clonar repositorio
```bash
git clone https://github.com/zXpect/gestor-recetas.git
```

---

### 📌 Conexión al remoto
```bash
git remote add origin https://github.com/zXpect/gestor-recetas.git
```

![Configuración remoto](gestor-recetas/docs/img/remote.png)

---

### 📌 Subir rama al repositorio
```bash
git push -u origin feature/recetas-italianas
```

![Push rama](gestor-recetas/docs/img/push.png)

---

### 📌 Actualizar ramas y verificar
```bash
git fetch --all
git branch -r
```

---

### 📌 Cambiar entre ramas
```bash
git checkout feature/recetas-italianas
git checkout main
```

---

### 📌 Agregar cambios en colombianas
```bash
git add gestor-recetas/recetas/colombianas.md
git commit -m "Agrego receta de arepas en colombianas.md"
git commit -m "Agrego variante de arepas en colombianas.md"
```

---

### 📌 Merge y resolución de conflictos
```bash
git merge feature/recetas-italianas
# Resolver conflicto en el archivo colombiano
git add gestor-recetas/recetas/colombianas.md
git commit -m "Resuelvo conflicto en colombianas.md unificando recetas de arepas"
```

![Conflicto y resolución](gestor-recetas/docs/img/checkout.png)

---

### 📌 Confirmaciones finales
```bash
git commit -m "Resuelvo conflicto en colombianas.md unificando recetas de arepas"
git push -u origin feature/recetas-italianas
```

---

### 📌 Trabajo con recetas colombianas
```bash
git restore gestor-recetas
git add gestor-recetas/gestor-recetas/
git commit -m "Adicion de 5 recetas colombianas"
git push -u origin feature/recetas-colombianas
git commit -m "Correccion de formato"
git push -u origin feature/recetas-colombianas
git commit -m "Adicion de notas"
git push -u origin feature/recetas-colombianas
```

---

### 📌 Creación y trabajo con recetas mexicanas
```bash
git checkout -b feature/recetas-mexicanas
git add gestor-recetas/recetas/mexicanas.md
git commit -m "Adicion 5 recetas mexicanas"
git push origin feature/recetas-mexicanas
git commit -m "Correccion Formato"
git push origin feature/recetas-mexicanas
git commit -m "Adicion de notas"
git push origin feature/recetas-mexicanas
```

---

## 🔹 3. Flujo de trabajo completado

1. Se creó la rama *feature/recetas-italianas*.  
2. Se añadieron varias recetas y se confirmaron los cambios.  
3. Se configuró el *remoto en GitHub*.  
4. Se realizaron *push* de las ramas al repositorio remoto.  
5. Se generaron *conflictos* al fusionar cambios en colombianas.md.  
6. Se resolvieron los conflictos unificando el contenido.
7. Se trabajó en la rama *feature/recetas-colombianas* agregando 5 recetas.
8. Se realizaron correcciones de formato y se añadieron notas adicionales.
9. Se creó la rama *feature/recetas-mexicanas* y se agregaron 5 recetas mexicanas.
10. Se aplicaron correcciones de formato y notas en las recetas mexicanas.