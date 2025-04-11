# Trabajo_Final_Churn

Este repositorio contiene un proyecto relacionado con la predicción de "Churn" utilizando datos específicos. A continuación, se describen los pasos necesarios para replicar este proyecto en tu entorno local utilizando Visual Studio Code.

## Requisitos previos

Antes de comenzar, asegúrate de tener instalados los siguientes programas y herramientas:

1. **Visual Studio Code**: [Descargar aquí](https://code.visualstudio.com/).
2. **Git**: [Descargar aquí](https://git-scm.com/).
3. **Python** (versión 3.8 o superior): [Descargar aquí](https://www.python.org/).
4. Extensiones recomendadas para Visual Studio Code:
   - Python (Microsoft)
   - GitLens (opcional, para manejo avanzado de Git)

## Pasos para replicar el proyecto

### 1. Clonar el repositorio

Abre una terminal en tu sistema operativo y ejecuta el siguiente comando para clonar este repositorio:

```bash
git clone https://github.com/Yesio11/Trabajo_Final_Churn.git
```

### 2. Abrir el proyecto en Visual Studio Code

1. Inicia Visual Studio Code.
2. Haz clic en **File** -> **Open Folder...**.
3. Navega hasta la carpeta donde clonaste el repositorio `Trabajo_Final_Churn` y selecciona la carpeta.

### 3. Crear y activar un entorno virtual

Recomendamos utilizar un entorno virtual para manejar las dependencias del proyecto. Sigue estos pasos:

1. Abre una terminal en Visual Studio Code (puedes usar **Ctrl+`**).
2. Ejecuta los siguientes comandos para crear y activar un entorno virtual:
   - En Windows:
     ```bash
     python -m venv venv
     venv\Scripts\activate
     ```
   - En macOS/Linux:
     ```bash
     python3 -m venv venv
     source venv/bin/activate
     ```

### 4. Instalar las dependencias

Con el entorno virtual activado, instala las dependencias necesarias ejecutando:

```bash
pip install -r requirements.txt
```

### 5. Configurar el proyecto

Verifica si existen archivos de configuración adicionales (como `.env` o configuraciones específicas). Si es necesario, crea dichos archivos siguiendo las instrucciones del repositorio o del equipo.

### 6. Ejecutar el proyecto

Ejecuta los scripts principales o notebooks del proyecto. Por ejemplo:

```bash
python main.py
```

O abre archivos `.ipynb` en Visual Studio Code y ejecuta las celdas.

### 7. Realizar cambios y usar Git

Si planeas realizar cambios en el proyecto y versionarlos, asegúrate de configurar Git en tu sistema. Los comandos básicos incluyen:

- **Preparar cambios**:
  ```bash
  git add .
  ```
- **Confirmar cambios**:
  ```bash
  git commit -m "Descripción de los cambios"
  ```
- **Subir cambios al repositorio remoto**:
  ```bash
  git push origin main
  ```

## Recursos adicionales

- [Documentación de Visual Studio Code](https://code.visualstudio.com/docs)
- [Documentación de Python](https://docs.python.org/3/)
- [Documentación de Git](https://git-scm.com/doc)

¡Listo! Siguiendo estos pasos podrás replicar el proyecto en tu entorno local utilizando Visual Studio Code.
```
