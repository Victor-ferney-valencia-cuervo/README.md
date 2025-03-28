- el juego elegido es: flappy bird 
- la funcion elegida es detectar cuando el pajaro choca contra los tubos 
### 1. algoritmo de la funcion del choque contra el tubo en pseint

```
Algoritmo Deteccion_Choque
    // Definir las coordenadas del pájaro
    Definir pajaro_x, pajaro_y Como Entero
    Definir ancho_pajaro, alto_pajaro Como Entero
    
    // Definir las coordenadas y dimensiones del tubo
    Definir tubo_x, tubo_y_superior, tubo_y_inferior Como Entero
    Definir ancho_tubo Como Entero
	
    // Asignar valores  
    pajaro_x = 100
    pajaro_y = 150
    ancho_pajaro = 30
    alto_pajaro = 30
	
    tubo_x = 120
    tubo_y_superior = 50
    tubo_y_inferior = 200
    ancho_tubo = 40
	
    // Verificar si el pájaro está alineado con el tubo en el eje X
    Si (pajaro_x + ancho_pajaro > tubo_x) Y (pajaro_x < tubo_x + ancho_tubo) Entonces
        // Verificar si hay colisión en el eje Y
        Si (pajaro_y < tubo_y_superior) O (pajaro_y + alto_pajaro > tubo_y_inferior) Entonces
            Escribir "¡Colisión detectada!"
        Sino
            Escribir "No hay colisión, el juego continúa."
        FinSi
    Sino
        Escribir "No hay colisión, el juego continúa."
    FinSi
FinAlgoritmo

```
### 2.pseudo codigo
```
nicio
    Definir posición del pájaro (x, y)
    Definir posición del tubo (x_tubo, y_tubo, ancho, alto)

    Si (pájaro.x + ancho_pájaro > tubo.x Y pájaro.x < tubo.x + ancho_tubo) Entonces
        Si (pájaro.y < tubo.y_superior O pájaro.y + alto_pájaro > tubo.y_inferior) Entonces
            Mostrar "¡Colisión detectada!"
        Fin Si
    Fin Si
Fin
```
### 3. diagrama de flujo



![image](https://github.com/user-attachments/assets/59382168-67bd-4925-93fb-5ff45da2776d)





