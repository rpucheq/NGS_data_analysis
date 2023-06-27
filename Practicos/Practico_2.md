# Ejercicio 2 - Archivos FASTQ, Control de Calidad y Ensamblaje de Genomas
## 1. Evaluar Calidad del FASTQ
### Descripción: 
FastQC es una herramienta de control de calidad para datos de secuenciación de alto rendimiento. Proporciona una manera rápida y fácil de evaluar la calidad de tus datos de secuenciación antes de realizar análisis posteriores.

Ademas, genera un informe en formato HTML que incluye gráficos y estadísticas sobre la calidad de tus datos. El informe incluye información sobre la calidad de las bases, la distribución del contenido de nucleótidos, la presencia de adaptadores y contaminantes, y otros aspectos importantes de la calidad de los datos.

Tambien es compatible con datos de secuenciación generados por diferentes tecnologías y puede analizar archivos en formato FASTQ, BAM y SAM. Es una herramienta útil para identificar problemas en tus datos de secuenciación y para asegurarte de que tus análisis posteriores se basen en datos de alta calidad.

### Comando para correr **FastQC**:
```bash 
fastqc archivo.fastq
```

Donde `archivo.fastq` es el archivo de lecturas que deseas analizar. FASTQC generará un informe en formato HTML con gráficos y estadísticas sobre la calidad de tus datos de secuenciación.

También puedes analizar múltiples archivos a la vez usando comodines. Por ejemplo:

```
fastqc *.fastq
```
Esto ejecutará FASTQC en todos los archivos con extensión `.fastq` en el directorio actual.


## 2. Ensamblaje usando SPAdes v3.11.1
### Descripción:
SPAdes (St. Petersburg genome assembler) es un software de ensamblaje de genomas desarrollado por la Universidad Académica de San Petersburgo de la Academia de Ciencias de Rusia en cooperación con científicos estadounidenses. Se utiliza principalmente para ensamblar pequeños genomas como bacterias y hongos.

SPAdes utiliza un enfoque de ensamblaje **de novo**, lo que significa que no requiere una secuencia de referencia para ensamblar el genoma. En su lugar, utiliza un algoritmo basado en gráficos para ensamblar las lecturas de secuenciación en contigs y scaffolds más largos.

SPAdes es capaz de manejar datos de secuenciación de diferentes tecnologías y puede utilizar múltiples conjuntos de datos para mejorar el ensamblaje. También incluye herramientas para corregir errores en las lecturas antes del ensamblaje.

En resumen, SPAdes es una herramienta poderosa y versátil para el ensamblaje de genomas pequeños a partir de datos de secuenciación.

### Comando para correr SPAdes:
```bash
spades.py --pe1-1 forward_reads.fastq --pe1-2 reverse_reads.fastq -o output_directory
```

Donde `forward_reads.fastq` y `reverse_reads.fastq` son tus archivos de lecturas paired-end y `output_directory` es el directorio donde deseas guardar los resultados del ensamblaje.

SPAdes tiene muchas opciones y parámetros que puedes ajustar para optimizar el ensamblaje. Puedes consultar la [documentación de SPAdes](https://github.com/ablab/spades) para obtener más información sobre cómo usar el programa. 
Sin usar un editor de texto (con interfaz grafica) 

