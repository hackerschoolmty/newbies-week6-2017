# Día 1, Lunes de Puente D:
## Recap OOP
https://docs.google.com/presentation/d/1iX405qniPk4KGNEo9f6iWC_t0eFgew9llgpJvFh4JTc/edit?usp=sharing

## Persistencia de Datos

Hasta el momento, los scripts y mini aplicaciones que hemos creado no han persistido los datos. La persistencia de datos es una funcionalidad fundamental para cualquier aplicación. ¿Se imaginan un facebook en donde tengan que volver a subir sus fotos cada que inician sesión?

En esta clase aprenderemos a trabajar con archivos para almacenar información y después poder leerla.

```python
with open('hello_world.txt', 'w') as f:
  f.write('hola mundo') #verificamos que exista un archivo con el nombre hello_world
# ¿como almacenamos la siguiente lista?
nombres = ['jesus', 'karen', 'alberto', 'miguel', 'cecilio']

# para leer el archivo hello_world
with open('hello_world.txt', 'w') as f:
  print(f.read())
# como podemos leer el archivo names.txt y mostrar linea por linea su contenido
```

###  Ejercicios Prácticos 1
1. Crea una clase que se encargue de buscar el nombre jesús en el archivo que acabamos de crear.
2. Crea un archivo con el contenido siguiente. Después crea una función que nos ayude a contar las veces que aparezca una palabra. Extra: ¿cómo lo haráis con una clase?

## CSV
Del Inglés ```comma separated values``` un archivo de este tipo permite almacenar información de forma estructurada. Tipicamente estos archivos toman la forma de un archivo de texto separado por coma y saltos de línea ```\n```

El siguiente es un archivo csv que contiene una lista de estudiantes

```csv
name, age, gender
jesus, 25, man
flor, 24, women
saul, 67, women
```
### Ejercicios prácticos 2
Toma como ejemplo el texto pasado para crear un archivo llamado ```students.csv``` carga este archivo en un programa de python y muestra cada uno con el siguiente formato. Nombre: Jesus, Edad: 23, Sexo: Hombre.
