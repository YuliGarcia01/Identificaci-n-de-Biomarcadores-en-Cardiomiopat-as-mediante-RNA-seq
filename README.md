# Identificación de Biomarcadores en Cardiomiopatías mediante RNA-
<img width="1517" height="912" alt="Cardiomyopathies" src="https://github.com/user-attachments/assets/63d3685a-e53b-413e-815f-a7e4ad122bd0" />

| Estatus | Lenguaje | Herramienta | Control de Versiones |
| :---: | :---: | :---: | :---: |
| 🟠 En Desarrollo | 🔵 R v4.x | 🟢 DESeq2 | 🔴 Git Activo |

## 📝 Propósito del Proyecto
Este proyecto de bioinformática surge con el propósito de analizar datos públicos de secuenciación de ARN de alto rendimiento (RNA-seq) provenientes de tejido cardíaco humano, tanto sano como patológico. A través de este análisis computacional, se busca explorar a fondo los mecanismos moleculares subyacentes a la insuficiencia cardíaca, permitiendo a investigadores y profesionales de la salud comprender mejor las alteraciones genéticas transcripcionales que impulsan el desarrollo de miocardiopatías.
## Fisiología 
Los biomarcadores en cardiomiopatías mediante RNA-seq se centra en cómo la expresión génica refleja los procesos celulares y tisulares que determinan la función cardíaca. El miocardio sano mantiene un equilibrio entre contractilidad, metabolismo energético, homeostasis del calcio y remodelado estructural; cuando este equilibrio se altera, aparecen patrones transcriptómicos característicos que pueden ser detectados por RNA-seq. En la cardiomiopatía dilatada, por ejemplo, se observa una desregulación de genes relacionados con el citoesqueleto, la matriz extracelular y la señalización inmunitaria, lo que se traduce en pérdida de fuerza contráctil y dilatación ventricular. En la cardiomiopatía hipertrófica predominan cambios en genes que regulan la hipertrofia celular, el metabolismo mitocondrial y la respuesta al estrés mecánico, generando engrosamiento de la pared y alteraciones en la relajación diastólica. En la restrictiva, los perfiles transcriptómicos muestran activación de vías de fibrosis y depósito de proteínas anómalas que limitan la distensibilidad ventricular. RNA-seq permite capturar estas modificaciones fisiológicas a nivel molecular, revelando cómo la inflamación, el estrés oxidativo y la remodelación estructural se integran en la progresión clínica. Así, los biomarcadores transcriptómicos no solo reflejan el estado funcional del corazón, sino que también anticipan la transición hacia insuficiencia cardíaca, ofreciendo una ventana fisiológica para diagnóstico temprano, estratificación de riesgo y diseño de terapias personalizadas.
## Interés clínico de los biomarcadores
Los biomarcadores derivados de RNA-seq en cardiomiopatías tienen un interés clínico creciente porque permiten identificar perfiles moleculares específicos asociados a diagnóstico temprano, pronóstico y potenciales dianas terapéuticas, superando las limitaciones de los métodos convencionales. En particular, se han validado genes y firmas transcriptómicas que distinguen subtipos de cardiomiopatía y predicen evolución hacia insuficiencia cardíaca. 
* Diagnostico temprano: RNA-seq permite detectar genes diferencialmente expresados en tejido miocárdico y células inmunes, incluso antes de que se manifiesten cambios estructurales o funcionales.
* Pronóstico y estratificación de riesgo: Firmas transcriptómicas permiten diferenciar pacientes con mayor riesgo de progresión a insuficiencia cardíaca.
* Integración con otras técnicas: RNA-seq se combina con imágenes cardíacas y biomarcadores de ARN no codificante (miRNAs, lncRNAs), mejorando la capacidad de estratificación clínica. 
* Potenciales diana terapéuticas: Los perfiles transcriptómicos revelan vías moleculares alteradas (ej. inflamación, remodelado extracelular, estrés oxidativo).
Estos hallazgos abren la puerta a nuevos tratamientos dirigidos según el perfil molecular del paciente.
## :book: Propósito del Repositorio 
El propósito de este repositorio es proporcionar una plataforma de trabajo colaborativo que permita a los integrantes del Equipo E desarrollar y documentar un proyecto de bioinformática. En este espacio se centralizan el código fuente, la documentación, los datos, los resultados y demás recursos necesarios para facilitar la organización, el control de versiones y la colaboración entre los miembros del equipo.

## 🎯 Objetivos del Análisis
*   *Identificar* genes diferencialmente expresados (DEGs) estadísticamente significativos al comparar muestras de tejido cardíaco sano frente a tejido con insuficiencia cardíaca.
*   *Detectar* rutas moleculares, ontologías génicas (GO) y procesos biológicos significativamente alterados en la muestra patológica.
*   *Descubrir* biomarcadores clave (firmas de expresión transcripcional) que tengan potencial uso clínico para el diagnóstico temprano y el diseño de terapias dirigidas.
*   *Implementar* un flujo de trabajo bioinformático reproducible y estandarizado en el lenguaje R utilizando paquetes de la suite Bioconductor.

## :dart: Objetivos generales
-Familiarizar a los estudiantes con el uso de Git y GitHub como herramientas de control de versiones y colaboración en proyectos de bioinformática.
-Enseñar a los estudiantes a crear un repositorio en GitHub y gestionar sus archivos y carpetas.
-Promover la colaboración y el trabajo en equipo a través de la creación de un repositorio compartido.
-Fomentar la presentación y el intercambio de proyectos de bioinformática entre los estudiantes.

## :dart: Objetivos particulares
- Plantear una metodología para el análisis de muestras genómicas con kits comerciales de generación de librerías y secuenciación de la casa comercial de Illumina

## 📂 Estructura Modular del Repositorio
Para cumplir con los estándares de reproducibilidad y ordenamiento del proyecto, el espacio de trabajo se organiza de la siguiente manera:
*   data/: Almacena de forma local las matrices de conteos genómicos crudos, archivos de índices y metadatos clínicos asociados a las muestras.
*   scripts/: Aloja exclusivamente el código fuente ejecutable en R (.R o .Rmd) encargado del procesamiento estadístico, filtrado y modelado de datos.
*   results/: Contiene los archivos de salida generados, incluyendo tablas tabuladas de genes significativos (.csv) y los reportes gráficos de control de calidad.
## :books: Estructura Modular del repositorio  

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
