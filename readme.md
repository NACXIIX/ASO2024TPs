# TP N°3 de Arquitectura y Sistemas operativos

## Punto 1

### a)

Con respecto al tiempo de ejecución de los archivos conhilos.py y sinhilos.py se puede notar que el programa conhilos es más rapido, esto se debe a que esta trabajando con hilos mediante la librería threading. En este caso en particular, en el programa conhilos.py, se puede observar que cada hilo trabaja en una funcion tarea diferente, es decir que empiezan y trabajan todas al mismo tiempo, dando a ello que el programa termine cuando finaliza la ultima tarea, por ello es mas rapido. Mientras que en el archivo sinhilos.py primero empieza la tarea 1, y la tarea 2 no empieza hasta que finalice la tarea 1, y asi lo mismo con la tarea 3 provocando de esta manera que el programa sea aún mas lento.
Esto es predecible ya que un programa que aborda multiples tareas simultaneamente es mas rápido y eficiente que una tarea que lo hace de manera secuencial.

### b)

Al comparar con mis compañeros puedo observar que mantenemos un mismo margen de tiempo, el unico cambio que veo es que en el archivo conhilos.py a algunos compañeros les finaliza las tareas en distinto orden.
Esto se puede deber a que en la tarea 1 al contener un bucle mi pc lo procese mas lento y es por ello que la tarea 1 termine mas tarde que la tarea 2.

### c)
Cuando las lineas 11, 12, 19 y 20 estan comentadas, es decir que no estan en funcionamiento, el valor final que nos da es 0, y el tiempo de ejecución es corto (0.10seg) . Cuando las lineas estan descomentadas y funcionan en el programa el tiempo de ejecución es mas largo de un aproximado de 17-20seg ya que se en esas lineas hay un bucle que se repite 1000 veces, este bucle a su vez se encuentra en otro bucle que ya esta repitiendose 100000 veces, es decir hay un bucle que se repite 1000 veces por cada vuelta del bucle que lo contiene. Ademas de lo anterior mencionado tambien el valor final ya deja de ser 0 y aparece un valor positivo o un valor negativo esto puede deberse a que al haber otro bucle dentro de otro las funciones de suma y resta no se sumen y resten secuencialmente una con otra como lo hacia con las lineas 11,22,19 y 20 comentadas.

## PUNTO 2

### a) 