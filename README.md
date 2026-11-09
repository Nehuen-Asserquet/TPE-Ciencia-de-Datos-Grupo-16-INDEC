# Trabajo Práctico Especial (TPE) - Fundamentos de la Ciencia de Datos (UNICEN 2026)

**Grupo 16** — Análisis de la **4° Encuesta Nacional de Factores de Riesgo (ENFR 2018 - INDEC)**.

---

## Estructura del Repositorio

* `TPE.ipynb`: Jupyter Notebook principal con el desarrollo completo del trabajo práctico (Análisis Exploratorio Inicial, Limpieza de Datos, Planteo de Hipótesis y Validación Estadística).
* `ENFR 2018 - Base usuario.txt`: Dataset original de la Encuesta Nacional de Factores de Riesgo 2018 provisto por el INDEC (separado por `|`).
* `requirements.txt`: Archivo con el listado de librerías y sus versiones necesarias para reproducir el entorno virtual.
* `.gitignore`: Configuración de archivos y carpetas excluidos del control de versiones (como el entorno virtual).

---

## Requisitos Previos

* Tener instalado **Python 3** en la computadora (Windows, Linux o macOS).
* Tener instalado **Git** (opcional, para clonar el repositorio).

---

## Instrucciones de Instalación y Ejecución Local

Siga estos pasos en orden desde una terminal (consola) para configurar el ambiente virtual y ejecutar la notebook localmente:

### 1. Clonar el repositorio y ubicarse en la carpeta del proyecto

Abra una terminal y ejecute:

```bash
git clone https://github.com/Nehuen-Asserquet/TPE-Ciencia-de-Datos-Grupo-16-INDEC.git
cd TPE-Ciencia-de-Datos-Grupo-16-INDEC
```

*(Nota: Asegúrese de que el archivo de datos `ENFR 2018 - Base usuario.txt` se encuentre en el mismo directorio raíz que `TPE.ipynb`).*

---

### 2. Crear el ambiente virtual (venv) con PIP

Para aislar las librerías del proyecto, cree un entorno virtual ejecutando:

```bash
python -m venv venv
```

*(Si en Linux/macOS el comando `python` no es reconocido, utilice `python3 -m venv venv`).*

---

### 3. Activar el ambiente virtual

Parado en la carpeta del proyecto, active el entorno virtual según su sistema operativo:

* **En Windows:**
  ```bash
  venv\Scripts\activate
  ```
* **En Linux / macOS:**
  ```bash
  source venv/bin/activate
  ```

*(Una vez activado, verá `(venv)` al comienzo de la línea en su terminal).*

---

### 4. Instalar las dependencias del proyecto

Con el ambiente virtual activado, instale la versión empaquetada de las librerías utilizando `requirements.txt`:

```bash
pip install -r requirements.txt
```

---

### 5. Ejecutar la Jupyter Notebook (`TPE.ipynb`)

Puede abrir y ejecutar el archivo `TPE.ipynb` de cualquiera de las siguientes dos formas vistas en la cursada:

#### Opción A: Usando Visual Studio Code (VSCode)
1. Abra la carpeta del proyecto en **VSCode**.
2. Abra el archivo `TPE.ipynb`.
3. En la esquina superior derecha, seleccione como **Kernel** el intérprete de Python correspondiente al entorno virtual recién creado (`venv`).
4. Ejecute las celdas secuencialmente o presione **Run All**.

#### Opción B: Usando Jupyter Notebook o JupyterLab desde el navegador
1. Con el entorno virtual activado, si aún no tiene instalado JupyterLab o Jupyter Notebook en su venv, instálelo corriendo:
   ```bash
   pip install jupyterlab
   ```
   *(o bien `pip install notebook`).*
2. Inicie el servidor interactivo ejecutando en la terminal:
   ```bash
   jupyter-lab
   ```
   *(o bien `jupyter notebook`).*
3. En la pestaña que se abrirá automáticamente en su navegador web, haga clic sobre **`TPE.ipynb`** y ejecute las celdas en orden de arriba hacia abajo.

---

### 6. Desactivar el ambiente virtual

Al finalizar la ejecución, puede desactivar el entorno virtual en cualquier sistema operativo ejecutando:

```bash
deactivate
```
