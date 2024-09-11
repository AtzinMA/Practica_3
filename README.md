# Práctica 3
## Integrantes
- Dante Mejía Silva
- Atzin Morales Alejandre



## Instrucciones

Primero, se analizó la trayectoria que debía seguir el robot Epson. Esta consistía en los siguientes pasos: inicialmente, el robot debía agarrar un fusible y colocarlo en una caja situada debajo de su brazo. Luego, debía tomar otro fusible, ubicado en el lado opuesto al del primer fusible, y colocarlo en la posición del primer fusible retirado. Finalmente, el fusible que se encontraba en la caja era nuevamente tomado para ser colocado en la posición del segundo fusible. 

<p align="middle"> 

 ![image](https://github.com/user-attachments/assets/11094b5b-daa7-4c24-b06b-29ccf2af4642) 
 
</p>

Con esta secuencia definida, se procedió a programar el robot utilizando el software Epson RC+, logrando el siguiente resultado:
```
Function main
Home
Go primero
On 2
Go segundo
Off 2
Go primero
Home
Go tercero
On 2
Go levantartres
Go cuarto
Go quinto
Off 2
Go cuarto
Home
Go primero
Go segundo
On 2
Go primero
Home
Go tercero
Off 2
Home
Go cuarto
Go quinto
On 2
Go cuarto
Home
Fend
```

