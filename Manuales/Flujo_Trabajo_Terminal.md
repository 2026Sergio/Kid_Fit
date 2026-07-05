#📝 Manual Técnico: Vinculación y Sincronización del Repositorio Upstream

En el flujo de trabajo colaborativo (Forking Workflow), el repositorio **upstream** hace referencia al repositorio central y original del proyecto (alojado en la cuenta de la organización o del líder del proyecto). 

Configurar correctamente el `upstream` te permite descargar las actualizaciones del equipo, evitar conflictos de código y mantener tu bifurcación (*fork*) totalmente sincronizada.

---

## 1. Configuración del Remoto Upstream

Realiza estos pasos desde la terminal integrada de Visual Studio Code (`Ctrl + Ñ` o `Ctrl + \``):

### Paso 1: Verificar los remotos actuales
Antes de agregar nada, comprueba qué conexiones tiene tu repositorio local ejecutando:
```bash
git remote -v
```

### Paso 2: Agregar el repositorio original como upstream
Vincula el repositorio central del proyecto utilizando el comando git remote add. (Reemplaza la URL de ejemplo con la URL real del proyecto KID-FIT):  
```bash
git remote add upstream (https://github.com/ORGANIZACION_O_LIDER/KID-FIT.git)
```
---
# Sincronización Diaria Obligatoria
Para evitar trabajar sobre código obsoleto y prevenir conflictos antes de programar una nueva característica, ejecuta esta secuencia exacta de comandos en tu terminal:

### Paso 1: Asegurar que estás en tu rama de desarrollo local
```bash
git checkout dev
```

### Paso 2: Traer el historial del repositorio original
Descarga toda la información del repositorio central sin modificar tus archivos locales actuales:
```bash
git fetch upstream
```

### Paso 3: Fusionar los cambios del upstream en tu rama local
Introduce los cambios de la rama dev del proyecto original en tu rama dev local:
```bash
git merge upstream/dev
```

### Paso 4: Actualizar tu repositorio en GitHub (Fork)
Sube los cambios que acabas de fusionar localmente a tu nube personal para que tu fork esté al día:
```bash
git push origin dev
```
