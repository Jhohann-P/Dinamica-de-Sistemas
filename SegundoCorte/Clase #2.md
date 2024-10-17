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

![Figura de prueba](images/plantilla/Captura2.PNG)

Figura 1. Figura de prueba

Incluya la respectiva etiqueta a modo de descripción de la figura y mantenga numeración consecutiva para todas las figuras de la clase.

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
Deben agregar 2 ejercicios con su respectiva solución, referentes a los temas tratados en cada una de las clases. Para agregar estos, utilice la etiqueta #, es decir como un nuevo título dentro de la clase con la palabra 'Ejercicios'. Cada uno de los ejercicios debe estar numerado y con su respectiva solución inmediatamente despues del enunciado. Antes del subtitulo de cada ejercicio incluya el emoji 📚

## 10. Conclusiones
En esta clase se abordaron los conceptos clave sobre el análisis de circuitos eléctricos en serie que contienen resistencias, inductores y capacitores. Se discutieron las ecuaciones diferenciales involucradas y su importancia para predecir el comportamiento del circuito en el tiempo. Además, se practicó la solución de estas ecuaciones y su implementación en MATLAB.

## 11. Referencias
Agregue un subtítulo al final donde pueda poner todas las referencias consultadas incluyendo el origen o fuente de los ejercicios planteados. Tambien dentro del texto referencie los textos o artículos consultados y las figuras y tablas dentro de la explicación de las mismas.
