# Práctica 3
## Integrantes
- Dante Mejía Silva
- Atzin Morales Alejandre



## Instrucciones

Primero, se analizó la trayectoria que debía seguir el robot Epson. Esta consistía en los siguientes pasos: inicialmente, el robot debía agarrar un fusible y colocarlo en una caja situada debajo de su brazo. Luego, debía tomar otro fusible, ubicado en el lado opuesto al del primer fusible, y colocarlo en la posición del primer fusible retirado. Finalmente, el fusible que se encontraba en la caja era nuevamente tomado para ser colocado en la posición del segundo fusible. Al mismo tiempo se guardaban todas la posiciones analizadas.

![Imagen de WhatsApp 2024-09-06 a las 21 07 07_ce4dab11](https://github.com/user-attachments/assets/fcbd7f5a-f674-4506-a0c9-0d850a1aba28)

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

Primeramente, se colocó el brazo en la posición de “Home”.

![image](https://github.com/user-attachments/assets/a9802f0f-37f8-452f-9dea-7b1c052624fb)

Después cuidadosamente tratando de evitar una colisión se movió el brazo a la posición “primero”, la cual corresponde al punto donde el brazo está encima del fusible, es decir, las coordenadas X y Y son las correctas, sin embargo, el brazo en la coordenada Z se encuentra desplazado un poco hacia arriba.

La posición “segundo” corresponde al punto donde el brazo toma el fusible, es decir, se coloca se disminuye en Z para bajar el brazo. Para tomar el brazo es necesario cerrar la pinza del brazo, esto mediante el comando “off 2”.

![Imagen de WhatsApp 2024-09-06 a las 21 07 07_e71102f8](https://github.com/user-attachments/assets/f7a782be-a488-47b8-ae2a-bee92c794c26)

Una vez tomado el fusible se regresa el brazo a la posición “primero” y después a “Home”.

Ahora, es necesario soltar el fusible encima de la caja, por lo que se toma la posición “tercero” la cual corresponde a donde el brazo se encuentra encima de la caja y posteriormente se suelta el fusible mediante el comando “on 2”.

![image](https://github.com/user-attachments/assets/5fdee821-d9a1-4b85-a74d-5a547e87f3c4)

Una vez ubicado el primer fusible encima de la caja es necesario alzar un poco el brazo, de esta manera evitamos tirar erroneamente al suelo el fusible.

Después cuidadosamente tratando de evitar una colisión se movió el brazo a la posición “cuarto”, la cual corresponde al punto donde el brazo está encima del segundo fusible, es decir, las coordenadas X y Y son las correctas, sin embargo, el brazo en la coordenada Z se encuentra desplazado un poco hacia arriba.

La posición “quinto” corresponde al punto donde el brazo toma el segundo fusible, es decir, se coloca se disminuye en Z para bajar el brazo. Para tomar el brazo es necesario cerrar la pinza del brazo, esto mediante el comando “off 2”.

Para finalizar se siguó en la misma sintonía de programación para continuar la trayectoria previamente analizada. Concretando con éxito una trayectoria más compleja y extensa utilizando el brazo robótico.




