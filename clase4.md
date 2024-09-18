# Sistemas mecánicos mas complejos
## 1. Caracteristicas principales de los sistemas mecánicos a manejar
Los sistemas mecánicos son conjuntos de componentes físicos que interactúan entre sí para generar, transmitir o transformar movimiento y fuerzas. 
Estos sistemas están diseñados para cumplir con una función específica, y su comportamiento se basa en los principios fundamentales de la mecánica, 
como la dinámica, la cinemática, y las leyes de Newton.  

Movimiento traslacional: Movimiento lineal en el espacio (por ejemplo, el desplazamiento de un pistón).  
Movimiento rotacional: Movimiento alrededor de un eje (por ejemplo, la rotación de una rueda o un engranaje).  

## 2. Definiciones  
>🔑*Grados de libertad:* Representan el número de movimientos independientes que un sistema o un objeto puede realizar en el espacio.  
>🔑*Posición angular:* La posición angular es una magnitud que describe la orientación o el ángulo de un cuerpo en rotación respecto a un punto o eje de referencia.  
>🔑*Sistema rotacional:* Es aquel en el que los elementos experimentan un movimiento de rotación alrededor de un eje fijo.

## 3. Ejemplos
💡Ejemplo 1: Modelamiento de 2 masas con 3 resortes  
![image](https://github.com/user-attachments/assets/8a5b33c2-88ff-4f6f-9181-b273461dd6d4)  
Diagrama de cuerpo libre de cada objeto: 
![image](https://github.com/user-attachments/assets/31868730-4514-4753-9496-ce3ab0af66b1)  
- Cuerpo 1  
𝑢 − 𝐹𝑅1 − 𝐹𝑅2 − 𝐹𝐹 = 𝑚1 ∗ 𝑎𝑚1  
$$u(t) - k_1 \cdot x_1(t) - k_2 \cdot (x_1(t) - x_2(t)) - b \cdot \frac{d(x_1(t) - x_2(t))}{dt} = m_1 \cdot \frac{d^2 x_1(t)}{dt^2}$$

Esta ecuación describe la dinámica de un sistema donde:
     - \( u(t) \) es una función de entrada.
     - \( k_1 \) y \( k_2 \) son constantes de rigidez.
     - \( b \) es el coeficiente de fricción.
     - \( m_1 \) es la masa del primer componente.
     - \( x_1(t) \) y \( x_2(t) \) representan las posiciones de los componentes en el sistema.

- Cuerpo 2  
𝐹𝑅2 + 𝐹𝐹 − 𝐹𝑅3 = 𝑚2 ∗ 𝑎𝑚2  
$$k_2 \cdot (x_1(t) - x_2(t)) + b \cdot \frac{d(x_1(t) - x_2(t))}{dt} - k_3 \cdot x_2(t) = m_2 \cdot \frac{d^2 x_2(t)}{dt^2}$$
Esta ecuación modela la interacción entre las posiciones \( x_1(t) \) y \( x_2(t) \) en el sistema.  
     - \( k_2 \) y \( k_3 \) son constantes de rigidez.
     - \( b \) es el coeficiente de fricción.
     - \( m_2 \) es la masa del segundo componente.
     - \( x_2(t) \) representa la posición del segundo componente.
 

💡Ejemplo 2: Sistemas rotacionales  
![image](https://github.com/user-attachments/assets/63256378-a221-4f96-a6a1-56c0d5c4463a)  
Diagrama de cuerpo libre:  
![image](https://github.com/user-attachments/assets/887b1b2c-717a-4e98-98c0-7414c1a72a75)  
**Ecuaciones para Análisis de Sistemas Rotacionales**

Las siguientes ecuaciones representan el modelo dinámico de un sistema rotacional y se utilizan para simulación y análisis. Estas ecuaciones permiten estudiar el comportamiento angular del sistema:

1. **Primera Ecuación:**  

   $$T - F_R - F_F = J \cdot \alpha$$

   - **Descripción**: Esta ecuación describe la dinámica rotacional del sistema, donde:
     - \( T \) es el par aplicado (torque).
     - \( F_R \) es la fuerza reactiva.
     - \( F_F \) es la fuerza de fricción.
     - \( J \) es el momento de inercia.
     - \( \alpha \) es la aceleración angular.

2. **Segunda Ecuación:**
   
   $$T(t) - F_F = J \cdot \alpha \quad \text{donde} \quad \alpha \text{ es la aceleración angular}$$

   - **Descripción**: Esta ecuación es una forma simplificada de la anterior, donde se destaca la relación entre el par aplicado, la fuerza de fricción, el momento de inercia y la aceleración angular.

4. **Tercera Ecuación:**  
$$T(t) - k \cdot \theta(t) - b \cdot \frac{d \theta(t)}{dt} = J \cdot \frac{d^2 \theta(t)}{dt^2}$$

   - **Descripción**: Esta ecuación describe la dinámica del sistema rotacional considerando el torque aplicado, la constante de rigidez \( k \), el coeficiente de fricción \( b \), y el momento de inercia \( J \). Aquí:
     - \( \theta(t) \) es la posición angular.
     - \( k \) es la constante de rigidez.
     - \( b \) es el coeficiente de fricción.
     - \( J \) es el momento de inercia.
     - \(\frac{d^2 \theta(t)}{dt^2}\) es la aceleración angular.


## 4. Conclusiones
El modelado matemático de sistemas mecánicos es importante para controlar su comportamiento en ingeniería, sin un modelamiento o diagrama de cuerpo libre,
las ecuaciones se complican un poco ya que no se sabria a que dirección actuan las fuerzas ademàs las ecuaciones diferenciales son clave para describir la dinámica 
tanto de movimientos traslacionales como rotacionales en los sistemas.
