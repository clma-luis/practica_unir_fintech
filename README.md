# Repo para EIEC - DevOps - UNIR

Este repositorio nos servirá para demostrar el uso de Git en la asignatura de EIEC y muchas cosas mas.

---

Los comandos del Makefile funcionarán en Linux y MacOS. En caso de usar Windows, necesitarás adaptarlos o ejecutarlos en una máquina virtual Linux.

## Ejecución

python3 main.py <filename> <dup>
  filename: **ruta** al fichero que contiene la lista de palabras, una por línea
  dup: **yes|no**, yes para eliminar palabras duplicadas, no para mantener la lista

# Parámetros:
filename → ruta al fichero con palabras (una por línea)

dup      → yes | no  (eliminar duplicados o no)
order    → asc | desc (orden ascendente o descendente) [OPCIONAL]

# EJEMPLOS

# 1. Orden ascendente eliminando duplicados
python3 main.py words.txt yes asc

# 2. Orden descendente sin eliminar duplicados
python3 main.py words.txt no desc

# 3. Solo con parámetros obligatorios (por defecto ascendente)
python3 main.py words.txt yes

# CREAR ARCHIVO DE PRUEBA

# Puedes crear un archivo de ejemplo así:
echo -e "banana\napple\norange\nbanana\ngrape" > words.txt

# RESULTADO ESPERADO

# El script:
 - Lee palabras desde el archivo
 - Opcionalmente elimina duplicados
 - Ordena la lista (asc o desc)
 - Imprime el resultado en consola
