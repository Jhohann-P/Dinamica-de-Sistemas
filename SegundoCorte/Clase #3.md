# Modelado y Análisis de Sistemas Hidráulicos, Térmicos y Electrónicos

En esta clase, analizamos tres tipos de sistemas: amplificadores electrónicos (no inversores),sistemas hidráulicos (tanques interconectados), y sistemas térmicos (transferencia de calor). Se emplea la metodología de modelado matemático utilizando las leyes de Kirchhoff y principios de la termodinámica para desarrollar ecuaciones diferenciales que describen el comportamiento de estos sistemas.


## 1. Definición del Amplificador No Inversor

En un amplificador no inversor, la señal de entrada se aplica directamente a la entrada no inversora del amplificador operacional, lo que significa que la señal de salida está en fase con la señal de entrada.

## 2. Aplicación de las leyes de Kirchhoff

>🔑 *Leyes de Kirchhoff:* Las leyes de Kirchhoff permiten analizar circuitos eléctricos determinando la relación entre las corrientes y voltajes en los diferentes nodos del circuito. En este caso, se utiliza para obtener las ecuaciones necesarias que describen el comportamiento del amplificador no inversor.

>🔑 *Impedancia de entrada:* La impedancia de entrada de un amplificador no inversor ideal tiende al infinito, lo que significa que prácticamente no fluye corriente hacia las entradas del amplificador.

>🔑 *Capacitancia Térmica:* La capacidad de un sistema para almacenar energía en forma de calor.
  
>🔑 *Resistencia Térmica:* La oposición al flujo de calor. Depende de la conductividad térmica del material y de la geometría del sistema.

>🔑 *Ecuación de Conservación de Energía:* La diferencia de la energía interna de un sistema está dada por el flujo de calor que entra y sale del sistema.

## 3. Modelo matemático del circuito

Utilizando las leyes de Kirchhoff y el modelo simplificado del amplificador operacional, se obtiene el siguiente esquema:

$$V^+ = V^-$$

Donde $V^+$ y $V^-$ representan las tensiones en las entradas no inversora e inversora del amplificador, respectivamente. La entrada de este amplificador se describe mediante el siguiente esquema:

![image](https://github.com/user-attachments/assets/78572acd-9a5f-4e09-b37c-73e3099ba60d)


Figura 1. Circuito simplificado del amplificador no inversor.  

### 3.1 Modelo Matemático de Transferencia de Calor

El flujo de calor $\dot{Q}$ entre dos cuerpos está dado por la ley de Fourier:

$$\dot{Q} = \frac{T_i - T_o}{R_\theta}$$

Donde:
- $T_i$ es la temperatura de entrada.
- $T_o$ es la temperatura de salida.
- $R_\theta$ es la resistencia térmica.

La variación de la temperatura de salida con el tiempo está dada por la ecuación:

$$C \frac{d T_o}{dt} = \frac{T_i - T_o}{R_\theta}$$  
## 4. Ejemplo

💡 **Ejemplo 1:** Supongamos que el amplificador tiene una ganancia de $A_v = 10$. Si la entrada $E_i(s)$ es de 1 V, la salida $E_o(s)$ será 10 V, ya que el amplificador no inversor amplifica la señal sin invertir su fase.

$$E_o(s) = A_v \cdot E_i(s)$$

## 5. Sistemas Hidráulicos

En la segunda parte de la clase, se analizaron sistemas hidráulicos, enfocándose en sistemas de tanques. Estos sistemas se modelan utilizando intercambios de masa y flujos de entrada y salida.

### 5.1. Sistemas de tanques

Los sistemas de tanques industriales buscan mantener el flujo constante o controlado. El flujo de salida se puede modelar como:

$$q_1 = \frac{h_1}{R_1}$$

Donde $q_1$ es el flujo, $h_1$ la altura del líquido en el tanque, y $R_1$ la resistencia hidráulica. El intercambio de masa entre tanques se modela mediante las ecuaciones de flujo y altura.

## 6. Sistemas Térmicos

Finalmente, se discutieron sistemas térmicos, con un enfoque en la capacidad calorífica y la transferencia de energía entre líquidos.

🔑 *Capacitancia térmica:* La capacitancia térmica es la capacidad de un sistema para almacenar energía en forma de calor. En un sistema térmico, se modela como una resistencia térmica en paralelo con una capacitancia.


## 7. Ejercicios y Soluciones

📚 **Ejercicio 1:** 

**Enunciado:** Modela el sistema de tanques mostrado en la figura de la clase. Encuentra la ecuación diferencial que describe el flujo $q_2$ en función de la resistencia $R_2$ y la altura $h_2$.

**Solución:**

El flujo de salida de un tanque está dado por la ley de la resistencia hidráulica:

$$ q_2 = \frac{h_2}{R_2} $$

Donde $h_2$ es la altura del líquido en el tanque y $R_2$ es la resistencia hidráulica. Ahora, aplicamos la ecuación de continuidad para la conservación de la masa en el tanque:

$$ \frac{d h_2}{dt} = \frac{q_1 - q_2}{A} $$

Donde $q_1$ es el flujo de entrada y $A$ es el área de la sección transversal del tanque. Sustituyendo el valor de $q_2$:

$$\frac{d h_2}{dt} = \frac{q_1 - \frac{h_2}{R_2}}{A}$$

Esta es la ecuación diferencial que describe el sistema de tanques en términos del flujo de entrada $q_1$, la altura $h_2$, y la resistencia $R_2$.

---

📚 **Ejercicio 2:** 

**Enunciado:** Para el sistema térmico mostrado en clase, encuentra la ecuación que relaciona el flujo de calor con la temperatura del líquido de entrada y salida, considerando la resistencia térmica $R_\theta$ y la capacitancia $C$.

**Solución:**

Para modelar un sistema térmico, usamos la ley de conservación de la energía. El flujo de calor $\dot{Q}$ está relacionado con la diferencia de temperatura y la resistencia térmica:

$$\dot{Q} = \frac{T_i - T_o}{R_\theta}$$

Donde $T_i$ es la temperatura de entrada, $T_o$ la temperatura de salida, y $R_\theta$ es la resistencia térmica. La tasa de cambio de la temperatura en el sistema está relacionada con el calor almacenado:

$$C \frac{d T_o}{dt} = \dot{Q}$$

Sustituyendo el valor de $\dot{Q}$ en esta ecuación:

$$C \frac{d T_o}{dt} = \frac{T_i - T_o}{R_\theta}$$

Esta es la ecuación diferencial que describe el sistema térmico en términos de la temperatura de entrada $T_i$, la temperatura de salida $T_o$, la resistencia térmica $R_\theta$, y la capacitancia térmica $C$.

## 8. Conclusiones

En esta clase, aprendimos a modelar el comportamiento de amplificadores no inversores, sistemas hidráulicos y térmicos utilizando las leyes de Kirchhoff y modelos simplificados. Esto nos permite entender mejor cómo los sistemas electrónicos, hidráulicos y térmicos pueden ser analizados y diseñados utilizando ecuaciones diferenciales y conceptos de física.

## 9. Referencias
https://amplificadores.info/amp-op/no-inversor
