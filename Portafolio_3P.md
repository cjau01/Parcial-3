# Presentacion 
## Problemas resueltos en clase con DFD
### Ejercicio 1.
#### 1.1 Analisis.
USANDO 2 VECTORES CAPTURE EDAD Y SEMESTRE DE N ESTUDIANTES
#### 1.2 DFD
![DIAGRAMA 1](https://user-images.githubusercontent.com/113397533/205477181-1b846a53-45c5-4f01-9e9c-2c34d3c3886e.jpg)
#### 1.3 Prueba de escritorio
corrida|valor i|V E|V S|i=n?|
|-|-|-|-|-|
|1|0|VE[0]=16|VS[0]=3|no|
|2|1|VE[1]=17|VS[1]=5|no|
|3|2|VE[2]=18|VS[2]=7|no|
|4|3|VE[3]=17|VS[3]=5|Si, impr VE y VS|

**Ejemplo**

|Edad|Semestre|
|-|-|
|16|3|
|17|5|
|18|7|
|17|5|

#### 1.4 Entradas.
sem| n| edad|

#### 1.5 Salidas.
"dame semestre entre [1,12]" | "¿cuantos estudiantes?" | "dame tu edad" | "fuer de rango" | "E,S"

### Ejercicio 2.
#### 1.1 Analisis. 
USANDO MATRICES CAPTURE EDAD Y SEMESTRE DE N ESTUDUANTES

#### 1.2 DFD
![DIAGRAMA 2](https://user-images.githubusercontent.com/113397533/205480999-4afc60b4-261b-4fb3-ab5f-77bd885f56d0.jpg)

#### 1.3 Prueba de escritorio
|corrida|valor i|valor j|matriz|i=n?|
|-|-|-|-|-|
|1|0|0|M[0,0]=16|no|
|2|1|0|M[1,0]=17|no|
|3|2|0|M[2,0]=17|no|
|4|3|0|M[3,0]=16|Si, entonces sig contador|

|corrida|valor i|valor j|matriz|i=n?|
|-|-|-|-|-|
|1|0|0|M[0,1]=3|no|
|2|1|0|M[1,1]=5|no|
|3|2|0|M[2,1]=5|no|
|4|3|0|M[3,1]=3|Si, entonces impr [M]|


**Ejemplo**

|Edad|Semestre|
|-|-|
|16|3|
|17|5|
|17|5|
|16|3|

#### 1.4 Entradas.
N| E| S| 

#### 1.5 Salidas.
"¿cuantos estudiantes?"| "fuera de rango"| "edad"| "semestre"| "no. de estudiante".: i+1, "edad": M[i,0], "semestre": m[i,1]|

### Ejercicio 3.
#### 1.1 Analisis. 
RELLENAR UNA MATRIZ CUADRADA (NxN) CON UN NUMERO LEIDO DEL TECLADO

#### 1.2 DFD

#### 1.3 Prueba de escritorio
|i|j|Matriz|num|i=M?|
|-|-|-|-|-|
|0|0|M[0,0|5|no|
|0|1|M[0,1]|7|no|
|0|2|M[0,2]|8|si, entonces J+1 y vuelve a empezar|

**Ejemplo**

|5|7|8|
|-|-|-|
|5|7|8|
|5|7|8|

#### 1.4 Entradas.
N| NUM|

#### 1.5 Salidas.

"¿TAMAÑO DE LA MATRIZ?"| "DAME NUM"| "DEBE SER MAYOR A 0"|

### Ejercicio 4.
#### 1.1 Analisis. 
RELLENAR UNA MATRIZ NxN CON NUMEROS CONSECUTIVOS
|1|2|3|
|-|-|-|
|4|5|6|
|7|8|9|
#### 1.2 DFD

#### 1.3 Prueba de escritorio
|i|j|Matriz|C|i=M?|
|-|-|-|-|-|
|0|0|M[0,0|0|no|
|0|1|M[0,1]|0|no|
|0|2|M[0,2]|0|si, entonces vuelve a empezar|

**Ejemplo**

|1|2|3|
|-|-|-|
|4|5|6|
|7|8|9|

#### 1.4 Entradas.
|N|

#### 1.5 Salidas.
|"TAMAÑO DE MATRIZ"| "DEBE SER MAYOR A 2 O MENOR-IGUAL A 100"

### Ejercicio 5.
#### 1.1 Analisis. 
RELLENE UNA MATRIZ DE NxN PER QUE REPITA TODO EL RENGLON EL MISMO NUMERO
|1|1|1|
|-|-|-|
|2|2|2|
|3|3|3|

#### 1.2 DFD

#### 1.3 Prueba de escritorio
|i|j|Matriz|C|i=M?|
|-|-|-|-|-|
|0|0|M[0,0|1|no|
|0|1|M[0,1]|1|no|
|0|2|M[0,2]|1|si, entonces C+1 y vuelve a empezar|

**Ejemplo**

|1|1|1|
|-|-|-|
|2|2|2|
|3|3|3|

#### 1.4 Entradas.
|N|

#### 1.5 Salidas.
|"TAMAÑO DE LA MATRIZ"| "FUERA DEL RANGO [100,100]"

### Ejercicio 6.
#### 1.1 Analisis. 
GENERE UNA MARIZ QUE QUEDE
|1|0|0|0|
|-|-|-|-|
|0|2|0|0|
|0|0|3|0|
|0|0|0|4|

#### 1.2 DFD

#### 1.3 Prueba de escritorio
Primero rellenamos 


|corridas|i|j|M|j=m?|
|-|-|-|-|-|
|1|0|1|M[0,0]=0|no|
|2|0|2|M[0,0]=0|no|
|3|0|3|M[0,0]=0|no|
|4|0|4|0|0|M[0,0]=0|si, entonces i+1 y j=0|

Ejemplo

|0|0|0|0|
|-|-|-|-|
|0|0|0|0|
|0|0|0|0|
|0|0|0|0|

Ahora hacemos la secuencia y en cada ciclo acabado le sumamos 1 a j

|Corridas|i|M|
|-|-|-|
|1|0|M[i,i=i+1|
|2|1|M[i,i=i+1|
|3|2|M[i,i=i+1|
|4|3|M[i,i=i+1|


Ejemplo

|1|0|0|0|
|-|-|-|-|
|0|2|0|0|
|0|0|3|0|
|0|0|0|4|

#### 1.4 Entradas.
|N|

#### 1.5 Salidas.
|"TAMAÑO DE LA MATRIZ"| "FUERA DEL RANGO [100,100]"

### Ejercicio 7.
#### 1.1 Analisis. 
CONVERTIR
|1|4|9|                      
|-|-|-|                     
|16|25|36|               
|49|64|81|  
    |
    V
 |1|
 |-|
 |4|
 |9|
 |16|
 |25|
 |36|
 |49|
 |64|
 |81|
#### 1.2 DFD

#### 1.3 Prueba de escritorio
|corridas|Matriz|Vector|j+1|
|-|-|-|-|
|1|M 0,0|M 0,0=V 0|j+1|
|2|M 0,1|M 0,1=V 1|j+1|
|3|M 0,2|M 0,2=V 2|j+1|

If j=M, i+1 and j=0 y regresa el ciclo hasta que i=M

Ejemplo 

|1|2|3|
|-|-|-|
|4|5|6|
|7|8|9|

Para

|1|
|-|
|2|
|3|
|4|
|5|
|6|
|7|
|8|
|9|

#### 1.4 Entradas.
|N|
#### 1.5 Salidas.
|"TAMAÑO DE LA MATRIZ"| "FUERA DEL RANGO [100,100]"| V[i]|

### Ejercicio 8.
#### 1.1 Analisis. 
EL 1B QUIERE CONOCER EL PROMEDIO POR PERSONA Y POR MATERIA, ADEMAS DE LA MATERIA CON MEJOR PROMEDIO GRUPAL Y AL ALUMNO CON MEJOR PROMEDIO, SON 7 MATERIAS 
Y 32 ALUMNOS, MENCIONE LOS ALUMNOS EN RIESGO (CON ALMENOS 1 MATERIA REPROBADA)
             a l u m n o s         
            |1|2|3|4|5|6|7| 
            |-|-|-|-|-|-|-|
            | | | | | | | |
#### 1.2 DFD

#### 1.3 Prueba de escritorio
|corridas|i|j|M|j+1|
|-|-|-|-|-|
|1|0|0|M 0,0=Materia|j+1|
|2|0|1|M 0,1=Materia|j+1|
|3|0|2|M 0,2=Materia|j+1|
|4|0|3|M 0,3=Materia|j+1|

If J=M, i+1 and j=0, y vuelve a iniciar ahora con calificaciones

Ejemplo 

|Español|Matematicas|Historia|Geografia|
|-|-|-|-|
|5|4|3|9|
|8|6|4|7|
|9|7|7|6|
|7|9|8|7|

#### 1.4 Entradas.
(ASIGNACION)
  M[33,7]
  VA[33]
  VM[7]
  
#### 1.5 Salidas.
|VA[i]| VM[i]| MM,MA| "ALUMNO EN RIESGO"|

### Ejercicio 9.
#### 1.1 Analisis. 
PREGUNTE LAS DIMENSIONES DE UNA MATRIZ EL RANGO ES [5,5], VALIDA QUE SEA CUADRADA Y OBTENGA LA SUMA DE LA DIAGONAL PREINCIPAL Y LA INVERSA.
  DETERMINE CUAL ES MAYOR, PREGUNTE LOS VALORES PARA LLENAR LA MATRIZ
  
#### 1.2 DFD

#### 1.3 Prueba de escritorio
  |corridas|j|M|j+1|
|-|-|-|-|
|1|0|M j,j+sig|j+1|
|2|1|M j,j+sig|j+1|
|3|2|M j,j+sig|j+1|

If j=M, impr Suma 

J=M

|corridas|j|M|j-1|
|-|-|-|-|
|1|0|M j,j+sig|j-1|
|2|1|M j,j+sig|j-1|
|3|2|M j,j+sig|j-1|

#### 1.4 Entradas.
| r| c|

#### 1.5 Salidas.
|"DAME EL NUMERO DE RENGLONES DE LA MARIZ"| "DAE EL NUMERO DE COLUMNAS"| "EL NUMERO DE COLUMNAS DEBE SER IGUAL AL DE LOS RENGLONES"
 |"FUERA DEL RANGO"| "DP ES MAYOR"| "DI ES MAYOR"| 
 
### Ejercicio 10.
#### 1.1 Analisis. 
ALMACENAR EN UN ARRAY LA SUMATORIA DE LOS NUMEROS DEL 1 HASTA N EN CADA POSICION DEL ARRAY, EJEMPLO SI N:3 (2,1) EL ARRAY DEBERA SER 1,3,6
|1|
|-|
|3|
|6|

#### 1.2 DFD

#### 1.3 Prueba de escritorio
|i|vector|i=V?|
|-|-|-|
|1|0|V[i]=V[i-1]+i+1|
|2|1|V[i]=V[i-1]+i+1|
|3|2|V[i]=V[i-1]+i+1|

Ejemplo

|1|
|-|
|3|
|6|

#### 1.4 Entradas.
|N|

#### 1.5 Salidas.
|"TAMAÑO DE ARRAY MENOR  100"| "N DEBE SER >0 Y <100"| "A"|

### Ejercicio 11.
#### 1.1 Analisis. 
DADA UNA MATRIZ DE NxM ALMACENAR EN UN VECTOR LAS MAYORES

#### 1.2 DFD

#### 1.3 Prueba de escritorio
|i|j|M|Suma|
|-|-|-|-|
|0|0|M [i,j]>mayor?-->si, M[i,j]=V [c] and C=c+1|j+1|
|0|1|M [i,j]>mayor?-->si, M[i,j]=V [c] and C=c+1|j+1|
|0|2|M [i,j]>mayor?-->si, M[i,j]=V [c] and C=c+1|j+1|
|0|3|M [i,j]>mayor?-->si, M[i,j]=V [c] and C=c+1|j+1|

If J=M, J=0 and I+1 y vuelve a iniciar

#### 1.4 Entradas.
|N| M| NUM|

#### 1.5 Salidas.
|"TU NUMERO DE RENGLONES"| "NUMERO DE COLUMNAS"| "FUERA DEL RANGO"| 
