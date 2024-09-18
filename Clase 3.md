# Sistemas Mecanicos
## 1. Principio General del Modelamiento
Existen 2 tipos de modelo  
- Modelo del balance de masa del sistema, Sistemas hidraulicos.  
- Modelo de balance de energia del sistema, Circuitos de Kirchoff   

Siempre se usa uno de estos tipos de balance que se obtiene
### 1.1 Sistemas Mecanicos
Se modelaran sistemas de resorte - amortiguador  
- Cuando se comprime o se estira un resorte se acumula energia pòtencial, lo cual produce una fuerza de reacción  
Lo cual nos dice la ley de hooke F= Kx = K(x1 - x2)  
Donde K es la constante y X1 y X2 es la distancia que se comprime o se estira el resorte
- Un amortiguador es un embolo que esta metido dentro de una carcasa, el amortiguador funciona por fricción viscosa va a productir una fuerza de reacción cuando intentemos desplazar el embolo  
F= bx = b(x'1-x'2)  
b = constante y x'1 y x'2 es la velocidad en la cual ocurrio eso  

## 2. Definiciones  
>🔑*Fricción en seco:* Es aquella cuando un cuerpo se desliza sobre una superficie no lubricada, o ambas no estan lubricadas (fricción estatica, deslizamiento, rodamiento)  
>🔑*Sistema Dinamico:* Un sistema se llama dinamico si su salida en el presente depende de una entrada en el pasado.  

## 3. Ejemplos.
Ejemplo 1.  
![image](https://github.com/user-attachments/assets/42a3fbad-29b6-4fe1-830e-6b44f4318bae)  

1. `u - F_R - F_F = m * a`

2. `u(t) - k2 * y(t) - F_F = m * a`

3. `F_R = k2 * y(t)`

4. `u(t) - k2 * y(t) - k1 * (dy(t) / dt) = m * a`

5. `F_F = k1 * (dy(t) / dt)`

6. `a = d^2 y(t) / dt^2`

7. `u(t) - k2 * y(t) - k1 * (dy(t) / dt) = m * (d^2 y(t) / dt^2)`

Ejemplo 2.  
Encontrar el modelo matemático para el Sistema que
representa la suspensión de un automóvil  
![image](https://github.com/user-attachments/assets/79ff02cd-c2a0-45ed-97ed-065f1c7139b3)  
Diagrama de cuerpo libre:  
![image](https://github.com/user-attachments/assets/f2034c06-ac32-4264-a883-49281fb91f5c)  

1. `Ef = M * A`

2. `u(t) + mg - Fr - Fa = M * a`

3. `u(t) + mg - K2 * Y(t) - K1 * y'(t) = M * y''(t)`




## 8. Conclusiones
El modelado de sistemas mecánicos permite predecir el comportamiento de componentes como resortes y amortiguadores mediante leyes físicas, facilitando el análisis de fuerzas y energía.
Los modelos de balance de masa y energía son esenciales en la representación de sistemas físicos, aplicables a diversos campos como la mecánica y los circuitos eléctricos.
