# Sistemas Eléctricos
## 1. Ecuaciones Diferenciales en Circuitos Eléctricos
Se introdujeron las ecuaciones diferenciales que gobiernan el comportamiento de los circuitos eléctricos en serie con resistencias (R), inductancias (L) y condensadores (C). El análisis se enfocó en la respuesta temporal del circuito.

### 1.1. Planteamiento de la Ecuación General
Se establece la ecuación de voltaje que describe la relación entre los componentes del circuito.

### 1.2. Solución de la Ecuación Diferencial
El siguiente paso es encontrar la solución a la ecuación diferencial planteada, para determinar el comportamiento del circuito a lo largo del tiempo.

## 2. Definiciones
>🔑 *Corriente Eléctrica (I):* es el flujo de carga eléctrica que pasa a través de un conductor por unidad de tiempo.

>🔑 *Voltaje (V):* es la diferencia de potencial eléctrico entre dos puntos de un circuito, lo que provoca el flujo de corriente.

>🔑 *Capacitor (C):* dispositivo que almacena energía en un campo eléctrico al acumular una diferencia de carga entre dos placas conductoras.
## 3. Subsecciones
### 3.1. Análisis de Circuito Serie RLC
Este análisis estudia el comportamiento de un circuito compuesto por una resistencia, un inductor y un condensador conectados en serie. La ecuación general para este sistema es una ecuación diferencial de segundo orden.

### 3.2. Circuitos con Resistencias y Capacitores (RC)
Aquí se describen circuitos en los que se combina una resistencia y un capacitor en serie, destacando cómo el voltaje y la corriente cambian con el tiempo.

## 4. Ejemplos
💡**Ejemplo 1:** Se plantea un circuito serie con una resistencia de 10Ω, un capacitor de 2F y una fuente de voltaje de 5V. Utilizando las leyes de Kirchhoff se desarrolla la siguiente ecuación diferencial para el sistema:

$$ V(t) = R \frac{dI}{dt} + \frac{1}{C} \int I \, dt $$

Se resuelve la ecuación para obtener la corriente en función del tiempo.

## 5. Ecuaciones
Para el análisis de los circuitos se utilizan las siguientes ecuaciones:

$$ V(t) = I R + L \frac{dI}{dt} + \frac{1}{C} \int I \, dt $$

Esta es la ecuación general para un circuito RLC en serie.

$$ I = C \frac{dV}{dt} $$

Esta es la relación entre la corriente y el voltaje en un capacitor.
## 6. Figuras
Todas las figuras que incluya deben ser generadas por ustedes, **no utilizar las figuras de las presentaciones**. Para incluir figuras puede seguir los siguientes pasos:
* Primero escribimos ![]().
* Después escribimos, dentro de los corchetes, el texto alternativo. Este es opcional y solo entra en acción cuando no se puede cargar la imagen correctamente.
* Después escribimos, dentro de los paréntesis, la ubicación del archivo (ya sea una url o una ubicación dentro de algun folder local). Se recomienda poner las imágenes en una carpeta que se llame imágenes dentro del repositorio github para que no tengan problemas al cargar las imágenes.

💡**Ejemplo 2:**

![image](https://github.com/user-attachments/assets/161c4f52-6dbe-44df-820b-f4a3d2195659)  
Figura 1. Representación del circuito RLC utilizado en el ejemplo.



## 7. Tablas
| Componente  | Valor    |
|-------------|----------|
| Resistencia | 10 Ω     |
| Capacitor   | 2 F      |
| Voltaje     | 5 V      |

Tabla 1. Valores de los componentes del circuito del Ejemplo 1.


## 8. Código
💡**Ejemplo 4:**
```matlab
% Código MATLAB para resolver la ecuación diferencial
syms I(t)
R = 10;
C = 2;
V = 5;
eqn = diff(I, t) + (1/(R*C)) * I == V/R;
sol = dsolve(eqn);
```

}

## 9. Ejercicios

### 📚 **Ejercicio 1:** 
Plantea un circuito serie con una resistencia de 5Ω y un capacitor de 1F conectado a una fuente de voltaje de 10V. Desarrolla la ecuación diferencial y resuélvela para determinar la corriente en el tiempo.

#### Solución:

1. **Ecuación del circuito**: Aplicando la ley de voltaje de Kirchhoff (KVL) al circuito:  

   $$V(t) = R \frac{dI}{dt} + \frac{1}{C} \int I \, dt$$

   Para los valores dados (R = 5Ω, C = 1F, V(t) = 10V):  

   $$10 = 5 \frac{dI}{dt} + \frac{1}{1} \int I \, dt$$  

2. **Derivando y simplificando**:   
   La ecuación se convierte en una ecuación diferencial de primer orden:  

   $$\frac{dI}{dt} + \frac{1}{5}I = 2$$  

3. **Resolviendo la ecuación diferencial**:    
   La solución homogénea es de la forma:  

   $$I_h(t) = Ce^{-t/5}$$  

   Para la solución particular, asumiendo que la corriente llega a un valor constante en el tiempo (cuando t → ∞), tenemos:  

   $$I_p(t) = 10$$  

4. **Solución general**:    
   La solución completa es la suma de la solución homogénea y particular:  

   $$I(t) = 10 + Ce^{-t/5}$$  

5. **Condiciones iniciales**:  
   Si inicialmente no hay corriente en el circuito (I(0) = 0):  

   $$0 = 10 + C \Rightarrow C = -10$$  

   Entonces, la solución final es:  

   $$I(t) = 10(1 - e^{-t/5})$$  

#### Respuesta:  
La corriente en función del tiempo es:  

$$I(t) = 10(1 - e^{-t/5}) \, \text{A}$$  
___

### 📚 **Ejercicio 2:**  
Para un circuito serie compuesto por una resistencia de 2Ω y un inductor de 0.5H, con una fuente de voltaje de 12V, desarrolla la ecuación diferencial correspondiente y resuélvela para encontrar el voltaje a través del inductor con respecto al tiempo.  

#### Solución:  

1. **Ecuación del circuito**: Aplicamos la ley de Kirchhoff:  

   $$V(t) = L \frac{dI}{dt} + R I$$  

   Para los valores dados (R = 2Ω, L = 0.5H, V(t) = 12V):  

   $$12 = 0.5 \frac{dI}{dt} + 2I$$  

2. **Reorganizando**:    
   La ecuación diferencial es:  

   $$\frac{dI}{dt} + 4I = 24$$  

3. **Resolviendo la ecuación diferencial**:  
   La solución homogénea es de la forma:

   $$I_h(t) = Ce^{-4t}$$  

   Para la solución particular, asumimos una corriente constante a largo plazo:  

   $$ I_p(t) = 6 $$  

4. **Solución general**:    
   La solución completa es:  

   $$ I(t) = 6 + Ce^{-4t} $$  

5. **Condiciones iniciales**:    
   Si inicialmente no hay corriente (I(0) = 0):  

   $$0 = 6 + C \Rightarrow C = -6$$  

   La solución final es:  

   $$I(t) = 6(1 - e^{-4t})$$  

6. **Voltaje en el inductor**:    
   El voltaje en el inductor es:  

   $$V_L(t) = L \frac{dI}{dt} = 0.5 \times 24 e^{-4t} = 12e^{-4t}$$  

#### Respuesta:  
El voltaje a través del inductor es:  

$$V_L(t) = 12 e^{-4t} \, \text{V}$$  


## 10. Conclusiones
En esta clase se abordaron los conceptos clave sobre el análisis de circuitos eléctricos en serie que contienen resistencias, inductores y capacitores. Se dieron a conocer las ecuaciones diferenciales involucradas. Además, se practicó la solución de estas ecuaciones.

## 11. Referencias
Agregue un subtítulo al final donde pueda poner todas las referencias consultadas incluyendo el origen o fuente de los ejercicios planteados. Tambien dentro del texto referencie los textos o artículos consultados y las figuras y tablas dentro de la explicación de las mismas.
