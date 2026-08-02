# Identificación de Biomarcadores en Cardiomiopatías mediante RNA-seq 
<img width="1517" height="912" alt="Cardiomyopathies" src="https://github.com/user-attachments/assets/63d3685a-e53b-413e-815f-a7e4ad122bd0" />

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

## 🎯 Objetivos Particulares
*   *Identificar* genes diferencialmente expresados (DEGs) estadísticamente significativos al comparar muestras de tejido cardíaco sano frente a tejido con insuficiencia cardíaca.
*   *Detectar* rutas moleculares, ontologías génicas (GO) y procesos biológicos significativamente alterados en la muestra patológica.
*   *Descubrir* biomarcadores clave (firmas de expresión transcripcional) que tengan potencial uso clínico para el diagnóstico temprano y el diseño de terapias dirigidas.
*   *Implementar* un flujo de trabajo bioinformático reproducible y estandarizado en el lenguaje R utilizando paquetes de la suite Bioconductor.

##  🎯 Objetivo general
Se busca integrar la fisiología cardíaca con la información molecular obtenida por RNA-seq, de modo que se traduzca en aplicaciones clínicas que mejoren la detección, la estratificación de riesgo y el diseño de intervenciones dirigidas, favoreciendo una visión continua y holística del paciente desde la biología básica hasta la práctica clínica. Así mismo, se pretende plantear una metodología para el análisis de muestras genómicas con kits comerciales de generación de librerías y secuenciación de la casa comercial de Ilumina. 

## 📂 Estructura de las carpetas del Repositorio
Para cumplir con los estándares de reproducibilidad y ordenamiento del proyecto, el espacio de trabajo se organiza de la siguiente manera:
*   data/: Almacena de forma local las matrices de conteos genómicos crudos, archivos de índices y metadatos clínicos asociados a las muestras.
*   scripts/: Aloja exclusivamente el código fuente ejecutable en R (.R o .Rmd) encargado del procesamiento estadístico, filtrado y modelado de datos.
*   results/: Contiene los archivos de salida generados, incluyendo tablas tabuladas de genes significativos (.csv) y los reportes gráficos de control de calidad.

## 🛠️ Instrucciones de Instalación y Uso

### Requisitos de Software
Es necesario contar con el entorno estadístico [R (versión 4.0 o superior)](https://r-project.org) y un entorno de desarrollo integrado compatible como RStudio.


## 📊 Resultados y Visualizaciones Esperadas
(Espacio reservado para el despliegue automático de las figuras analíticas definitivas del proyecto tras procesar las muestras de dicho proyecto)

El pipeline generará gráficos avanzados de diagnóstico molecular. Un ejemplo del formato de salida esperado para identificar la magnitud del cambio de expresión frente a su significancia estadística (Volcano Plot) se ilustra a continuación:

<img width="577" height="577" alt="Captura de pantalla 2026-07-31 191846" src="https://github.com/user-attachments/assets/61bed249-9225-4e8c-ae6b-ccc78fbfbf2f" />


## 🔗 Enlaces de Interés y Documentación Científica
*   [Guía de referencia rápida de sintaxis Markdown (CheatSheet)](https://github.com)
*   [Flujo de análisis y documentación del paquete DESeq2 (Vignette)](https://bioconductor.org)
*   [Base de datos pública NCBI GEO (Gene Expression Omnibus)](https://nih.gov)
*   [Identification and multi-layered validation of seven diagnostic biomarkers for dilated cardiomyopathy via integrative machine learning, single-cell transcriptomics, and Mendelian randomization – Front Cell Dev Biol, 2026] (pubmed.ncbi.nlm.nih.gov in Bing)
*   [Single-nucleus RNA sequencing in ischemic cardiomyopathy reveals common transcriptional profile underlying end-stage heart failure – Cell Reports, 2023](pubmed.ncbi.nlm.nih.gov in Bing)
*  [Identification of potential dilated cardiomyopathy-related targets by meta-analysis and co-expression analysis of human RNA-sequencing datasets – Life Sciences, 2022] (pubmed.ncbi.nlm.nih.gov in Bing)
