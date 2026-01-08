# 🍷 Wine Quality ETL Pipeline & Analysis

Este proyecto implementa un pipeline de extracción, transformación y carga (ETL) para el dataset **Wine Quality** (Vinho Verde) del UCI Machine Learning Repository. 

El objetivo principal no es solo el análisis de datos, sino la **automatización robusta de la ingesta** y la preparación de estructuras de datos tanto para entornos SQL como NoSQL, aplicando principios de ingeniería de software a la ciencia de datos.

## 🚀 Características Clave

* **Ingesta Automatizada:** En lugar de descargas manuales, el script utiliza `BeautifulSoup` y `Requests` para localizar dinámicamente el enlace de descarga más reciente y procesarlo.
* **Manejo en Memoria:** Uso de `io` y `zipfile` para descomprimir y leer los datos directamente en memoria sin generar archivos en disco.
* **Manejo de Errores:** Implementación de bloques `try/catch` para asegurar la resiliencia del pipeline ante fallos de red o cambios en la estructura web.
* **Dual Storage Strategy:** Persistencia en los datos:
    * **SQL (SQLite):** Para consultas relacionales.
    * **NoSQL (MongoDB):** Estructuración de documentos JSON para bases de datos documentales.

## 🛠️ Stack Tecnológico
* **Python 3.x**
* **ETL & Data Manipulation:** Pandas, Numpy
* **Web Scraping & Ingesta:** Requests, BeautifulSoup4, Zipfile
* **Visualización:** Matplotlib, Seaborn
* **Bases de Datos:** SQLite3, JSON (se podría utilizar para MongoDB)

## 📋 Prerrequisitos e Instalación

> 💡 **Recomendación:** Para evitar conflictos con las versiones de librerías de tu sistema operativo o de otros proyectos, se recomienda encarecidamente utilizar un **entorno virtual**.

1.  Crear y activar el entorno virtual:
    * **Windows:**
        ```bash
        python -m venv venv
        .\venv\Scripts\activate
        ```
    * **Mac/Linux:**
        ```bash
        python3 -m venv venv
        source venv/bin/activate
        ```
1.  Clonar el repositorio:
    ```bash
    git clone [https://github.com/TU_USUARIO/pc1-etl-wine-quality.git](https://github.com/TU_USUARIO/pc1-etl-wine-quality.git)
    cd pc1-etl-wine-quality
    ```

2.  Instalar dependencias:
    ```bash
    pip install -r requirements.txt
    ```

## ⚙️ Cómo ejecutar

Abre el Jupyter Notebook para ver el flujo paso a paso:

```bash
jupyter notebook PC1_Wine_Quality.ipynb
