# Ejercicios - Linea de Comandos (Flash mode)

## Navegar por el sistema de archivos
1. Imprime tu directorio de trabajo actual con el comando `pwd`.
2. Crea un directorio en tu carpeta usando el comando `mkdir`
3. Entra al directorio recién creado usando `cd`
4. Puedes ver cuantos archivos existen usando `ls`

## Descargar el archivo desde la carpeta `Genomes` ubicado en Github:
1. Para descargar copia el siguiente comando:
   
   ```bash
   wget --no-check-certificate https://github.com/rpucheq/NGS_data_analysis/tree/main/Genomes
   ```
2. El archivo de trabajo es *Lborgpetersenii1.txt*

## Examina el contenido de: `Lborgpetersenii1.txt` usando `less` o `more`, y emplea los comandos indicados a continuación: 

## 1. `wc` nos permite:
- ¿Cuántas líneas contienen?
- ¿Cuántos caracteres?

## 2. Usando `head` y `tail`
- ¿Cuál es la primera línea de los archivos?
- ¿Cuáles son las 10 últimas? Puedes usar `tail`

## 3. Practica usando `>` o `>>` 
- Agregar la informacion de los pasos 1 y 2 nuevo archivo llamado `informacionLB.txt`
