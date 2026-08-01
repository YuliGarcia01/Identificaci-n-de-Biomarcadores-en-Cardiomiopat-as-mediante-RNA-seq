# Identificación de Biomarcadores en Cardiomiopatías mediante RNA-
<img width="1517" height="912" alt="Cardiomyopathies" src="https://github.com/user-attachments/assets/63d3685a-e53b-413e-815f-a7e4ad122bd0" />

| Estatus | Lenguaje | Herramienta | Control de Versiones |
| :---: | :---: | :---: | :---: |
| 🟠 En Desarrollo | 🔵 R v4.x | 🟢 DESeq2 | 🔴 Git Activo |

## 📝 Propósito del Proyecto
Este proyecto de bioinformática surge con el propósito de analizar datos públicos de secuenciación de ARN de alto rendimiento (RNA-seq) provenientes de tejido cardíaco humano, tanto sano como patológico. A través de este análisis computacional, se busca explorar a fondo los mecanismos moleculares subyacentes a la insuficiencia cardíaca, permitiendo a investigadores y profesionales de la salud comprender mejor las alteraciones genéticas transcripcionales que impulsan el desarrollo de miocardiopatías.

## 🎯 Objetivos del Análisis
*   *Identificar* genes diferencialmente expresados (DEGs) estadísticamente significativos al comparar muestras de tejido cardíaco sano frente a tejido con insuficiencia cardíaca.
*   *Detectar* rutas moleculares, ontologías génicas (GO) y procesos biológicos significativamente alterados en la muestra patológica.
*   *Descubrir* biomarcadores clave (firmas de expresión transcripcional) que tengan potencial uso clínico para el diagnóstico temprano y el diseño de terapias dirigidas.
*   *Implementar* un flujo de trabajo bioinformático reproducible y estandarizado en el lenguaje R utilizando paquetes de la suite Bioconductor.

## 📂 Estructura Modular del Repositorio
Para cumplir con los estándares de reproducibilidad y ordenamiento del proyecto, el espacio de trabajo se organiza de la siguiente manera:
*   data/: Almacena de forma local las matrices de conteos genómicos crudos, archivos de índices y metadatos clínicos asociados a las muestras.
*   scripts/: Aloja exclusivamente el código fuente ejecutable en R (.R o .Rmd) encargado del procesamiento estadístico, filtrado y modelado de datos.
*   results/: Contiene los archivos de salida generados, incluyendo tablas tabuladas de genes significativos (.csv) y los reportes gráficos de control de calidad.

## 🛠️ Instrucciones de Instalación y Uso

### Requisitos de Software
Es necesario contar con el entorno estadístico [R (versión 4.0 o superior)](https://r-project.org) y un entorno de desarrollo integrado compatible como RStudio.

### Instalación de Dependencias
Abre la consola de R y ejecuta los siguientes comandos para instalar el gestor BiocManager y las librerías necesarias para el modelado matemático y visualización de datos:

r
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

# Instalación de paquetes bioinformáticos y utilidades de graficación
BiocManager::install(c("DESeq2", "clusterProfiler", "org.Hs.eg.db"))
install.packages(c("ggplot2", "tidyverse", "EnhancedVolcano"))


### Flujo de Ejecución del Script
diff
+ 1. Realiza un Fork de este repositorio y clona la copia resultante en tu máquina local.
+ 2. Genera los archivos en tu explorador y obtén su dirección de origen local mediante "Copy Path".
+ 3. Deposita la matriz de conteos genómicos crudos y su archivo de metadatos dentro del directorio data/.
+ 4. Ejecuta el archivo principal de análisis para realizar la normalización y el contraste estadístico.


Para correr el script de forma directa desde la terminal del sistema operativo, navega hasta la raíz del proyecto y ejecuta:
bash
Rscript scripts/analisis_deseq2.R


## 📊 Resultados y Visualizaciones Esperadas
(Espacio reservado para el despliegue automático de las figuras analíticas definitivas del proyecto tras procesar las muestras)

El pipeline generará gráficos avanzados de diagnóstico molecular. Un ejemplo del formato de salida esperado para identificar la magnitud del cambio de expresión frente a su significancia estadística (Volcano Plot) se ilustra a continuación:

<img width="577" height="577" alt="Captura de pantalla 2026-07-31 191846" src="https://github.com/user-attachments/assets/61bed249-9225-4e8c-ae6b-ccc78fbfbf2f" />


## 🔗 Enlaces de Interés y Documentación Científica
*   [Guía de referencia rápida de sintaxis Markdown (CheatSheet)](https://github.com)
*   [Flujo de análisis y documentación del paquete DESeq2 (Vignette)](https://bioconductor.org)
*   [Base de datos pública NCBI GEO (Gene Expression Omnibus)](https://nih.gov)
