# Practica_9
## Integrantes:  
- Francisco Javier Godinez Lopez
- Pablo Axel Silva Fuentes
- Eduardo David Salas Ayala
- 
## Introducción:  

El objetivo de la práctica es ubicar una serie de fusibles dentro de los contenedores o charolas con la medida especfica de dichos fusibles, implementando un nuevo comando "CP" que tiene por fin, tener una trayectoria continua , definida por varios puntos, para realizar movimientos mas fluidos y precisos.

## Instrucciones

El robot Epson debe ubicar 6 fusibles dentro de una matriz 3x2.

1. Realizar el codigo utilizando los puntos guardados.
2. Con el robot, tomar ambas charolas y colocarlas en el punto asignado. 
3. Seleccionar la serie de fusibles a tomar lasa se colocadas en las charolas.
4. Ajustar la altura y presicion para la colocacion.
5. Comprobar posibles coliciones.
6. Ejecutar la programacion para realizar la tarea asignada.

De tal manera que el codigo desarrollado quedo de la siguiente manera:

```
Function main
	Reset
	Motor On
	Power High
	Speed 40

Home
On 2
Go Caja_Der_4, Caja_Der_3, Caja_Der_2 CP
Go Caja_Der_1
Off 2
Go Caja_Der_2, Caja_Der_3, Caja_Der_4 CP

Go Centro

Go Base1_4, Base1_3, Base1_2 CP
Go Base1_1
On 2
Go Base1_2, Base1_3, Base1_4 CP

Go Centro

Go Caja_Izq_4, Caja_Izq_3, Caja_Izq_2 CP
Go Caja_Izq_1
Off 2
Go Caja_Izq_2, Caja_Izq_3, Caja_Izq_4 CP

Go Centro

Go Base2_4, Base2_3, Base2_2 CP
Go Base2_1
On 2
Go Base2_2, Base2_3, Base2_4 CP

Go Centro

Go Fusible1_izq_4, Fusible1_izq_3, Fusible1_izq_2 CP
Go Fusible1_izq_1
Off 2
Go Fusible1_izq_2, Fusible1_izq_3, Fusible1_izq_4 CP

Go Centro

Go Base1_Fus_Izq_4, Base1_Fus_Izq_3, Base1_Fus_Izq_2 CP
Go Base1_Fus_Izq_1
On 2
Go Base1_Fus_Izq_2, Base1_Fus_Izq_3, Base1_Fus_Izq_4 CP

Go Centro

Go Fusible2_izq_4, Fusible2_izq_3, Fusible2_izq_2 CP
Go Fusible2_izq_1
Off 2
Go Fusible2_izq_2, Fusible2_izq_3, Fusible2_izq_4 CP

Go Centro

Go Base1_Fus_Der_4, Base1_Fus_Der_3, Base1_Fus_Der_2 CP
Go Base1_Fus_Der_1
On 2
Go Base1_Fus_Der_2, Base1_Fus_Der_3, Base1_Fus_Der_4 CP

Go Centro

Go Fusible1_Der_4, Fusible1_Der_3, Fusible1_Der_2 CP
Go Fusible1_Der_1
Off 2
Go Fusible1_Der_2, Fusible1_Der_3, Fusible1_Der_4 CP

Go Centro
 
Go Base2_Fus_Izq_4, Base2_Fus_Izq_3, Base2_Fus_Izq_2 CP
Go Base2_Fus_Izq_1
On 2
Go Base2_Fus_Izq_2, Base2_Fus_Izq_3, Base2_Fus_Izq_4 CP

Go Centro

Go Fusible2_Der_4, Fusible2_Der_3, Fusible2_Der_2 CP
Go Fusible2_Der_1
Off 2
Go Fusible2_Der_2, Fusible2_Der_3, Fusible2_Der_4 CP

Go Centro

Go Base2_Fus_Der_4, Base2_Fus_Der_3, Base2_Fus_Der_2 CP
Go Base2_Fus_Der_1
On 2
Go Base2_Fus_Der_2, Base2_Fus_Der_3, Base2_Fus_Der_4 CP

Go Centro
Home

Fend

```


En el siguiente video, se muestra cómo el robot Epson cumple con la tarea asignada, utilizando el nuevo mando para un movimiento mas fluidos, ademas de presciso, completando la tarea.



https://github.com/user-attachments/assets/0cd52b48-1009-4d87-b303-65cebae45b35


## Conclusiones:  
### Francisco Javier Godinez Lopez:
La práctica permitió trabajar en una tarea que exigía movimientos precisos y fluidos, lo que llevó al uso del comando "CP" como solución óptima. Este comando demostró su eficacia al permitir al robot seguir una trayectoria a través de puntos definidos, manteniendo suavidad y exactitud en todo momento. La experiencia resaltó la importancia de una programación bien diseñada para maximizar el rendimiento del robot y alcanzar resultados ideales. En este contexto, se reafirmó el valor de los robots en la ejecución de tareas técnicas avanzadas, donde la precisión es un factor clave para el éxito.


### Pablo Axel Silva Fuentes: 
En esta práctica, se llevó a cabo una tarea que demandaba tanto precisión como fluidez en los movimientos del robot. Esto permitió explorar y aplicar el comando "CP", diseñado para seguir trayectorias definidas por puntos almacenados previamente. Su implementación destacó la capacidad del robot para ejecutar movimientos continuos con gran exactitud, siempre que se programe de manera adecuada. Este ejercicio evidenció cómo los robots son herramientas fundamentales para realizar actividades complejas que requieren alta precisión, optimizando procesos y mejorando la eficiencia en aplicaciones específicas.


### Eduardo David Salas Ayala: 
En esta práctica, se realizó una tarea que requería alta precisión y fluidez en el movimiento del robot. Para ello, se aprendió y utilizó el comando "CP", cuya función es permitir al robot seguir una trayectoria a través de varios puntos previamente guardados. Durante su ejecución, se pudo observar cómo este comando respetó sus características al proporcionar movimientos suaves y precisos. Además, se destacó la importancia de una programación correcta para lograr resultados óptimos en tareas específicas. Esta experiencia permitió comprender la gran utilidad de los robots en la ejecución de trabajos complejos que demandan un alto nivel de precisión y eficiencia.


## Referencias bibliográficas
- Epson (2020). EPSON RC+ 7.0 Manual del usuario Administración y desarrollo de proyectos (Ver.7.3). https://files.support.epson.com/far/docs/epson_rc_pl_70_users_guide_spanish_(v73r2).pdf
