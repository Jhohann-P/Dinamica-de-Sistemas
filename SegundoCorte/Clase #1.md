# Energía Cinética y Potencial en Sistemas Mecánicos
En esta clase, se explora la relación entre las fuerzas y las energías que actúan sobre un cuerpo en movimiento. La energía cinética, que depende de la velocidad de un objeto, y la energía potencial, que depende de la posición de un objeto en un campo de fuerzas, como un resorte o un sistema conservativo, son los conceptos principales. Además, se discutirán aplicaciones prácticas de estos principios en sistemas con resortes y masas, así como en circuitos eléctricos análogos.

## 1. Subtítulos
1.1. Energía Cinética 1.2. Potencia 1.3. Aplicación de la Energía Potencial en un Resorte 1.4. Potencia en una Masa 1.5. Energía Dissipada y Sistema Conservativo 1.6. Recomendaciones para Sistemas Simples 1.7. Analogía con Circuitos Eléctricos RLC

## 2. Definiciones
🔑 Energía cinética: Es la energía asociada a un objeto debido a su movimiento. Está determinada por la velocidad y la masa del objeto.

🔑 Potencia: La variación del trabajo respecto al tiempo. Es una medida de cuánta energía se transfiere o transforma en un sistema por unidad de tiempo.

🔑 Energía potencial en un resorte: Es la energía almacenada debido a la deformación de un resorte. Se puede expresar como $U = \frac{1}{2}kx^2$, donde $k$ es la constante del resorte y $x$ la deformación.

## 3. Subsecciones
Se define como la energía asociada con el movimiento de un cuerpo. La fórmula básica de la energía cinética es:  
T = 1/2mv^2  
Donde $m$ es la masa del cuerpo y $v$ es la velocidad.  
3.2. Potencia
La potencia en un sistema mecánico se relaciona con la tasa de cambio de la energía o trabajo con respecto al tiempo:  
P = DW/DT
3.3. Aplicación en un Resorte
La energía almacenada en un resorte está dada por la siguiente fórmula, que representa la energía potencial elástica:  
U=1/2kx^2  
Donde $k$ es la constante del resorte y $x$ es la deformación.  

## 4. Ejemplos
💡Ejemplo 1:  

Dado un sistema con un resorte, calcular la energía potencial almacenada si la constante del resorte es $k = 200 , N/m$ y la deformación es $x = 0.05 , m$.  
Solución: U=(1/2)(200)(0.05)^2=0.25J  

💡Ejemplo 2:

Un bloque de masa $2 , kg$ se mueve con una velocidad de $3 , m/s$. Calcular su energía cinética.  

Solución: T=1/2(2)(3)^2=9J  

💡Ejemplo 3:  
![image](https://github.com/user-attachments/assets/b12052ab-1391-42bb-9fd5-b9b8cd60d8e7)  
Energía Total del Sistema Conservativo  
  
La energía total \( T + U \) se mantiene constante:  
  
$$T + U = \frac{1}{2} m \dot{x}^2 + \frac{1}{2} k x^2 = \text{constante}$$  
  
Donde:  
- \( m \) es la masa.  
- \( \dot{x} \) es la velocidad de la masa.  
- \( k \) es la constante del resorte.  
- \( x \) es la posición de la masa.  
  
Derivación de la Energía Total  
  
Al derivar la energía total con respecto al tiempo, obtenemos:  
$$\frac{d}{dt}(T + U) = m \ddot{x} \dot{x} + k x \dot{x} = (m \ddot{x} + k x) \dot{x} = 0$$  
Por lo tanto, la ecuación de movimiento es:  
$$m \ddot{x} + k x = 0$$  

## 5. Ecuaciones
Energía Cinética  
La energía cinética de un cuerpo está dada por la ecuación:  
$$T = \frac{1}{2} m v^2$$  

Potencia  
La potencia es la derivada del trabajo respecto al tiempo:  
$$P = \frac{dW}{dt}$$  

Trabajo Realizado por un Resorte  
El trabajo realizado por las fuerzas en un resorte se calcula como:  
$$W = \int_{0}^{x} F \, dx = \int_{0}^{x} Kx \, dx = \frac{1}{2} K x^2$$

Potencia en un Resorte  
La potencia en un resorte está dada por:  
$$P = \frac{dW}{dt} = F \dot{x} = K x \dot{x}$$  

Energía Potencial en un Resorte  
La energía potencial almacenada en un resorte es:  
$$U = \frac{1}{2} K x^2$$  

Energía Disipada en un Amortiguador  
La energía disipada por un amortiguador con coeficiente de fricción $b$ se puede expresar como:
$$\Delta W = \int_{x_1}^{x_2} b \dot{x} \, dx = b \int_{x_1}^{x_2} \dot{x}^2 \, dt = b \int_{\dot{x}_1}^{\dot{x}_2} \dot{x}^2 \, dt$$  



## 6. Figuras
Figura 1. Representación de un sistema masa-resorte.

## 7. Tablas

| Parametros            | Simbolos | Unidades |
|-----------------------|----------|----------|
| Constante del resorte | $k$      | N/m      |
| Velocidad             | $v$      | m/s      | 
| Masa                  | $m$      | KG       | 

## 8. Código
💡**Matlab:**
```
% Código para calcular la energía cinética
m = 2; % masa en kg
v = 3; % velocidad en m/s
T = 0.5 * m * v^2;
disp(T); % Muestra la energía cinética
```

## 9. Ejercicios
📚Ejercicio 1: Energía Cinética de una Masa  
Enunciado:  
Calcula la energía cinética de un cuerpo de masa $m$ = 5kg  que se mueve a una velocidad de 
$𝑣$=10m/s
Solución:
La fórmula para la energía cinética es:  
$$T = \frac{1}{2} m v^2$$  
Sustituyendo los valores:  
$$T = \frac{1}{2} \cdot 5 \, \text{kg} \cdot (10 \, \text{m/s})^2 = 250 \, \text{J}$$  


📚Ejercicio 2: Energía Potencial en un Resorte  
Enunciado:  
Determina la energía potencial almacenada en un resorte con una constante  
$𝐾$=200N/m y una deformación de x=0.1m.  

Solución:  
La energía potencial en un resorte está dada por:  
$$U = \frac{1}{2} K x^2$$  
Sustituyendo los valores:  
$$U = \frac{1}{2} \cdot 200 \, \text{N/m} \cdot (0.1 \, \text{m})^2 = 1 \, \text{J}$$  


📚Ejercicio 3: Potencia Disipada en un Amortiguador  
Enunciado:  
En un sistema con un amortiguador de coeficiente de fricción b=50N, calcula la energía disipada cuando la velocidad inicial es  
x'= 2m/s y la velocidad final es de x2'=0m/s  
Solución:  
La energía disipada está dada por:  
$$\Delta W = \int_{x_1}^{x_2} b \dot{x}^2 \, dt = b \int_{\dot{x}_1}^{\dot{x}_2} \dot{x}^2 \, dt$$  
Sustituyendo los valores:  
$$\Delta W = 50 \, \text{N·s/m} \cdot \left( \frac{2^2}{2} - \frac{0^2}{2} \right) = 100 \, \text{J}$$


## 10. Conclusiones
En esta clase hemos aprendido los conceptos fundamentales de energía cinética y energía potencial, aplicados principalmente a sistemas de masa-resorte. Estos conceptos son clave para entender el comportamiento dinámico de los sistemas mecánicos y sus aplicaciones prácticas en la ingeniería. También hemos visto cómo la energía se disipa en sistemas con fricción, y cómo estos principios son aplicables en diferentes áreas, como los circuitos eléctricos.

## 11. Referencias
Dinámica de sistemas, Ogata, K., Prentice 
Hall, 1987

