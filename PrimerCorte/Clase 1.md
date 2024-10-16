# Presentación del curso
## 1. Objetivos del curso
Identificar la simbología usada en la representación de sistemas (mecánicos, hidraulicos, 
eléctricos) para aplicarla en la elaboración de planos y diagramas.  
Reconocer los tipos de modelamiento y el uso para el análisis de sistemas.  
### 1.1 Metodología
Se realizaran clases presenciales teoricas, si se llegan a presentar acontecimientos que impidan llegar a la escuela o dia de virtualidad, se hará la clase mediante la plataforma en TEAMS

## 2. Definiciones  
>🔑*Sistema:* Es una combinación de componentes que actuan conjuntamente para alcanzar un objetivo especifico, la combinación de componentes se puede relacionar por medio de reglas o principios.  
>🔑*Sistema Dinamico:* Un sistema se llama dinamico si su salida en el presente depende de una entrada en el pasado.  

## 3. Dinamica de Sistemas.
Las subsecciones pueden utilizarse para sub dividir ciertos temas que se tienen en clases, por ejemplo si se está trabajandolos conversores D/A, puede ser necesario subdividir este en circuito de resistencias ponderadas y circuito de escalera R2R. 
### 3.1. Temas del curso
- Pre Requisitos:  
  Ecuaciones diferenciales
- Software:  
  Matlab  
  Simulador de circuitos
- Contenido:  
  Definiciones  
  Solución de ecuaciones diferenciales (transformada de laplace)
- Modelamiento matematico:
  Mecanicos  
  Electricos  
  Hidraulicos  
  Termicos
- Diagrama de bloques:
  Algebla de bloques  
  Diagrama de flechas (Formula de mason)  
  
  
### 3.2. Bibliografía
Se usarán los siguienes libros como referencia a lo largo de todo el curso.  
Libros básicos:  
Dinámica de Sistemas 1ra Edición Katsuhiko Ogata.  
Ingenieria de control moderna katsuhiko Ogata.  
Libros complementarios:  
Control automático de procesos: teoría y práctica Libro de Armando B. Corripio y Carlos A. Smith.  
### 3.2. Evaluación del curso
Autoevaluación y coevaluación : 20%  
Parcial: 40%  
Tareas: 30%  
Apuntes: 10%  
  -Plantilla.  
  -2 Ejercicios.  
  -Github.  
### 3.3. Matlab
Es un computo de programación númerico, el cual ofrece distintas tareas conforme a la programación matematica, su nombre se deriva de MATrix LABoratory o Laboratorio de matrices).  
Su sistema se maneja mediante lenguaje de programación unico o propio "Lenguaje M",
Figura 1.
## 4. Ejemplos
💡Ejemplo 1: Suma de matrices  
A = [7 8 2; 3 2 6; 5 9 4]  
B = [1 5 2; 6 7 9; 4 7 3]  
Se establecío la matriz a y b, cada una de estas con sus respectivos datos separados medianamente por una coma dando asi a las filas.  
Realizando la suma  
C = A + B  
💡Ejemplo 2: Resta de matrices  
Si fuera una resta:  
A = [7 8 2; 3 2 6; 5 9 4]  
B = [1 5 2; 6 7 9; 4 7 3]  
D= A-B    

## 5. Figuras
Figura 1.
![MATLAB](images/plantilla/matlab.JPG)


## 6. Código
>> A = [7 8 2; 3 2 6; 5 9 4];  
>> determinant_A = det(A);  
>> disp(determinant_A);  
  -144  

>> B = [1 5 2; 6 7 9; 4 7 3];  
>> inverse_B = inv(B);  
>> disp(inverse_B);  
   -0.5526   -0.0132    0.4079  
    0.2368   -0.0658    0.0395  
    0.1842    0.1711   -0.3026  

## 7. Ejercicios
📚 Determinante de una matriz:  
A = [7 8 2; 3 2 6; 5 9 4];  
determinant_A = det(A);  
disp(determinant_A);  
![image](images/plantilla/CapturaS.JPG)  
📚 Inversa de una matriz:  
B = [1 5 2; 6 7 9; 4 7 3];  
inverse_B = inv(B);  
disp(inverse_B);  
![image](images/plantilla/CapturaSo.JPG)  

## 8. Conclusiones
Se realizarón los acuerdos y se establecierón los prefijos para las reglas de calificación, se dió a conocer el syllabus como tema para conllevar a lo largo de el curso y los diferentes materiales de apoyo, siendo asi como libros y sistemas de abreviación matematica como MATLAB.

