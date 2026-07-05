# Manual Técnico: Creación de Ramas y Envío de Pull Requests (PR)

Este manual detalla el procedimiento estándar comando por comando para crear ramas de trabajo locales en Visual Studio Code, registrar tus cambios y enviarlos correctamente para que sean integrados en la rama `dev` del repositorio central.

---

## Paso a Paso: Crear una Rama de Trabajo Local

Antes de escribir cualquier línea de código, debes crear una rama aislada. Nunca trabajes directamente sobre `dev` o `main`.

### Paso 1: Posicionarte en la rama de desarrollo base
Asegúrate de estar parado en tu rama `dev` local:
```bash
git checkout dev
```

### Paso 2: Sincronizar tu entorno antes de ramificar
Descarga los últimos cambios del proyecto original para asegurarte de que tu nueva rama salga desde el código más reciente:
```bash
git pull upstream dev
```

### Paso 3: Crear y cambiarte a la nueva rama
Crea tu rama de característica utilizando una nomenclatura clara y profesional (ej. feature/calculadora-imc, feature/formulario-contacto):
```bash
git checkout -b nombre_rama
```

# Guardar y Subir los Cambios en VS Code

### Paso 1: Verificar el estado de tus archivos
Revisa qué archivos creaste, modificaste o eliminaste:
```bash
git status
```

### Paso 2: Agregar los cambios al área de preparación (Staging)
Prepara todos los archivos modificados para el commit:
```bash
git add .
```

### Paso 3: Confirmar los cambios localmente
Guarda tus cambios en el historial local con un mensaje claro siguiendo las buenas prácticas convencionales (Conventional Commits):
```bash
git commit -m "feat: "
```

### Paso 4: Subir la rama a tu repositorio remoto (Fork)
Publica tu rama local en tu fork personal de GitHub (origin):
```bash
git push origin feature/nombre-de-tu-tarea
```

