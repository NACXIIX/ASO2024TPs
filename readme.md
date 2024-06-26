# TP N°3 de Arquitectura y Sistemas Operativos

## Punto 1

### a)

Con respecto al tiempo de ejecución de los archivos conhilos.py y sinhilos.py se puede notar que el programa conhilos es más rapido, esto se debe a que esta trabajando con hilos mediante la librería threading. En este caso en particular, en el programa conhilos.py, se puede observar que cada hilo trabaja en una funcion tarea diferente, es decir que empiezan y trabajan todas al mismo tiempo, dando a ello que el programa termine cuando finaliza la ultima tarea, por ello es mas rapido. Mientras que en el archivo sinhilos.py primero empieza la tarea 1, y la tarea 2 no empieza hasta que finalice la tarea 1, y asi lo mismo con la tarea 3 provocando de esta manera que el programa sea aún mas lento.
Esto es predecible ya que un programa que aborda multiples tareas simultaneamente es mas rápido y eficiente que una tarea que lo hace de manera secuencial.

### b)

Al comparar con mis compañeros puedo observar que mantenemos un mismo margen de tiempo, el unico cambio que veo es que en el archivo conhilos.py a algunos compañeros les finaliza las tareas en distinto orden.
Esto se puede deber a que en la tarea 1 al contener un bucle mi pc lo procese mas lento y es por ello que la tarea 1 termine mas tarde que la tarea 2.

### c)
Las funciones sumador y restador alojadas una en cada hilo, trabajan sobre una variable global llamada acumulador, esta variable global es la region crítica ya que las dos funciones compiten por el mismo recurso generando de esta manera una race condition.
Cuando las lineas 11, 12, 19 y 20 estan comentadas, el valor final que nos da es 0, y el tiempo de ejecución es corto (0.10seg) pero como no hay ningun mecanismo de control se genera una race condition. Cuando las lineas estan descomentadas y funcionan en el programa el tiempo de ejecución es mas largo de un aproximado de 17-20seg ya que en esas lineas hay un bucle que se repite 1000 veces, este bucle a su vez se encuentra en otro bucle que ya esta repitiendose 100000 veces, es decir hay un bucle que se repite 1000 veces por cada vuelta del bucle que lo contiene. Ademas de lo anterior mencionado tambien el valor final ya deja de ser 0 y aparece un valor positivo o un valor negativo esto se debe a que con las lineas descomentadas el race condition es mucho mas evidente y los resultados inesperados son mas visibles. Debido a esta race condition el resultado puede ser cualquier numero.

## PUNTO 2

#### Imagen del punto 2.a) funcionando: 

![Punto2aOK](https://github.com/NACXIIX/ASO2024TPs/blob/main/TP3/IMAGENES/punto2a_funcionando.png)
El codigo se encuentra resuelto en la carpeta TP3/

#### Imagen del punto 2.b):

![Punto2bOK](https://github.com/NACXIIX/ASO2024TPs/blob/main/IMAGENES/grafico_comensales.png)





# TP N°4 de Arquitectura y Sistemas Operativos

#### Imagen del punto a)
![PuntoAOK](https://github.com/NACXIIX/ASO2024TPs/blob/main/IMAGENES/TP4_A_docker-compose-s_servicios_creados_corriendo.png)

#### Imagen del punto b)
![PuntoBOK](https://github.com/NACXIIX/ASO2024TPs/blob/main/IMAGENES/TP4_B_phpmyadmin_y_nginx.png)

#### Imagen del punto c)
![PuntoCOK](https://github.com/NACXIIX/ASO2024TPs/blob/main/IMAGENES/TP4_C_facultadlocalhost.png)