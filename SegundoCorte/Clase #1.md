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
Ejemplo 1:

Dado un sistema con un resorte, calcular la energía potencial almacenada si la constante del resorte es $k = 200 , N/m$ y la deformación es $x = 0.05 , m$.
Solución: U=(1/2)(200)(0.05)^2=0.25J

Ejemplo 2:

Un bloque de masa $2 , kg$ se mueve con una velocidad de $3 , m/s$. Calcular su energía cinética.

Solución: T=1/2(2)(3)^2=9J

## 5. Ecuaciones
Para la edición de ecuaciones debe utilizar la etiqueta '$$' al comienzo y final de la ecuación para que la ecuación quede centrada ocupando una línea. Si se quiere que la ecuación quede integrada en el texto debe utilizar la etiqueta '$' al comienzo y final de la ecuación. Las ecuaciones pueden ser editadas utilizando el código LATEX, en el siguiente enlace encuentran un editor de ecuaciones que les genera el código. http://www.alciro.org/tools/matematicas/editor-ecuaciones.jsp . Sin embargo hay muchas otras herramientas que pueden utilizar para esto.

💡**Ejemplo 1:** si se va a representar la ecuación de la ley de Ohm se puede mostrar así $R=\frac{V}{I}$ o también,

$$R=\frac{V}{I}$$

## 6. Figuras
Todas las figuras que incluya deben ser generadas por ustedes, **no utilizar las figuras de las presentaciones**. Para incluir figuras puede seguir los siguientes pasos:
* Primero escribimos ![]().
* Después escribimos, dentro de los corchetes, el texto alternativo. Este es opcional y solo entra en acción cuando no se puede cargar la imagen correctamente.
* Después escribimos, dentro de los paréntesis, la ubicación del archivo (ya sea una url o una ubicación dentro de algun folder local). Se recomienda poner las imágenes en una carpeta que se llame imágenes dentro del repositorio github para que no tengan problemas al cargar las imágenes.

💡**Ejemplo 2:**

Figura 1. Figura de prueba

Incluya la respectiva etiqueta a modo de descripción de la figura y mantenga numeración consecutiva para todas las figuras de la clase.

## 7. Tablas

| Parametros            | Simbolos | Unidades |
|-----------------------|----------|----------|
| Constante del resorte | $k$      | N/m      |
| Velocidad             | $v$      | m/s      | 
| Masa                  | $m$      | KG       | 

Tabla 1. Tabla de ejemplo

Cada tabla debe llevar la etiqueta que describa su contenido y numeración consecutiva para todas las tablas

## 8. Código
% Código para calcular la energía cinética
m = 2; % masa en kg
v = 3; % velocidad en m/s
T = 0.5 * m * v^2;
disp(T); % Muestra la energía cinética


💡**Ejemplo 4:**
```
var sumar2 = function(numero) {
  return numero + 2;
}
```

## 9. Ejercicios
Ejercicio 1: Energía Cinética de una Masa  
Enunciado:
Calcula la energía cinética de un cuerpo de masa $m$ = 5kg  que se mueve a una velocidad de 
$𝑣$=10m/s
Solución:
La fórmula para la energía cinética es:  
$$ T = \frac{1}{2} m v^2 $$  
Sustituyendo los valores:  
$$ T = \frac{1}{2} \cdot 5 \, \text{kg} \cdot (10 \, \text{m/s})^2 = 250 \, \text{J} $$  


## 10. Conclusiones
En esta clase hemos aprendido los conceptos fundamentales de energía cinética y energía potencial, aplicados principalmente a sistemas de masa-resorte. Estos conceptos son clave para entender el comportamiento dinámico de los sistemas mecánicos y sus aplicaciones prácticas en la ingeniería. También hemos visto cómo la energía se disipa en sistemas con fricción, y cómo estos principios son aplicables en diferentes áreas, como los circuitos eléctricos.

## 11. Referencias
Agregue un subtítulo al final donde pueda poner todas las referencias consultadas incluyendo el origen o fuente de los ejercicios planteados. Tambien dentro del texto referencie los textos o artículos consultados y las figuras y tablas dentro de la explicación de las mismas.
