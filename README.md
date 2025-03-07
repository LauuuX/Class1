# Clase #1 Definiciones 
## En dinámica de sistemas, se analizan los sistemas como conjuntos de componentes que interactúan para alcanzar un objetivo, depende de entradas y salidas. 
## 1. Sistema
>  🔑 Un sistema es una combinación de componentes que actúan conjuntamente para alcanzar un objetivo específico. La combinación de componentes se puede representar por medio de reglas o principios que relacionan las salidas con las entradas.
![Sistema ](https://github.com/user-attachments/assets/65ca1914-d9bc-4330-a279-ce7039b7a6ef)
> 
Figura 1. Sistema 
## 2. Sistemas dinámicos 
> 🔑 Un sistema es una porción de la realidad que se selecciona para su estudio y modelado. Cuando dicho sistema experimenta cambios a lo largo del tiempo, se le denomina sistema dinámico. Para representar su evolución, se utilizan modelos dinámicos, los cuales consisten en funciones matemáticas que describen el comportamiento del sistema en función del tiempo. Estos modelos permiten predecir su estado futuro y analizar la relación entre sus variables, facilitando su comprensión y control en diversas aplicaciones.
![Sistema dinámico](https://github.com/user-attachments/assets/86efcfa7-db6d-440d-9bd9-985eec7bffac)
> 
Figura 2. Ejemplo de sistema dinámico  
## 3. Planta 
> 🔑 Componente físico o proceso que se desea controlar o modelar. Es el sistema en sí mismo, sin incluir los elementos de control o medición. La planta puede estar representada por ecuaciones matemáticas que describen su comportamiento en función del tiempo y las entradas que recibe.

![Planta](https://github.com/user-attachments/assets/6fe83d46-aa8b-4328-9833-6f33abf9c304)

Figura 3. Planta  
## 4. Proceso 
> 🔑 Proceso es la secuencia de cambios o transformaciones que ocurren dentro de la planta para convertir una entrada en una salida. Representa la evolución del sistema en el tiempo y puede describirse mediante modelos matemáticos que expresan la relación entre las variables involucradas. En el contexto del control de sistemas, el proceso es el fenómeno que se desea regular o mejorar para alcanzar un comportamiento deseado.

![Proceso](https://github.com/user-attachments/assets/369dc4e6-2339-451f-addd-ef09b2d36302)

Figura 4. Proceso
## 5. Modelos dinámicos
> 🔑 El modelo dinámico describe aquellos aspectos de un sistema relacionados con el tiempo y la secuencia de operaciones : eventos que marcan cambios, secuencias de eventos y la organización de eventos y estados. El modelo dinámico no considera qué hacen las operaciones, sobre qué operan ni cómo se implementan.

![Modelo dinámico](https://github.com/user-attachments/assets/bb9fa61c-3860-4144-bec3-03d9728dfe2f)

Figura 5. Modelo dinámico

### 5.1 En control interesa obtener un modelo matemático que relacione las variables de intéres con el tiempo 
$$f(t)$$
### 5.2 Es necesario cuantificar cuanto cambia las variables de interés con respecto al tiempo 
$$\frac{df\left(t\right)}{dt}$$
# 6. Modelos de ecuaciones diferenciales
## Son combinaciones lineales de derivadas de diferente orden
$${a_1\ \frac{d^2F}{at}+\ a_2\frac{dF}{dt}\ +\ a_3F\ =\ u\left(t\right)}$$
* Donde F es la salida del sistema
* Donde U es la entrada del sistema
* La solución no es un número es una función
## 6.1 Características de una ecuación diferencial 
* Ecuación lineal invariante en el tiempo
  
$$\frac{d^2x\left(t\right)}{dt^2}+5\frac{dx\left(t\right)}{dt}+10x\left(t\right)=0$$
  
* Ecuación lineal variante en el tiempo
  
$$\frac{d^2x\left(t\right)}{dt^2}+\left(1-\cos \left(2t\right)\right)\ x\left(t\right)=0$$

* Ecuación no lineal variante en el tiempo

$$\frac{d^2x\left(t\right)}{dt^2}+\left(x^2\left(t\right)-1\right)\ \frac{dx\left(t\right)}{dt}+x\left(t\right)=0$$

* Ecuación no lineal invariante en el tiempo

$$\frac{d^2x\left(t\right)}{dt^2}+\ \frac{dx\left(t\right)}{dt}+x\left(t\right)\ +\ x^3\left(t\right)=sen\left(wt\right)$$

## 6.2 Sistemas lineales y no lineales 
* Un sistema se considera lineal cuando cumple con el principio de superposición
   * La respuesta de un sistema al que se le aplican dos o más excitaciones simultáneas, es la suma de las respuestas individuales.
* Un sistema lineal también tiene la característica de proporcionalidad entre la entrada y la salida.
* Los sistemas no lineales no cumplen con el principio de superposición.
* Los sistemas no lineales se linealizan en un punto de operación, en el cual se cumple el principio de superposición.
## 6.3 Modelamiento y validación
* Al aplicar leyes físicas a un modelo matemático de un sistema, se debe tener en cuenta que hay un nivel de incertidumbre en el resultado final.
* Es necesario validar el modelo con respecto al sistema físico comparando la salida del modelo con la salida del modelo físico, si no es aceptable la diferencia se debe modificar el modelo hasta conseguir una diferencia aceptable.

## 6.3 Influencia de parámetros
* Comportamiento de un oscilador armónico (senoidal)
  
  ![image](https://github.com/user-attachments/assets/ce44de6f-003c-4b13-99c6-b811794a9aea)
  
Figura 6. Oscilador 
