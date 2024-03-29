# APUNTES DE LA PRIMERA PARCIAL
## Programación Funcional
***Algunos paradigmas de programación:***     
a) Paradigma imperativo. Indica el procedimiento paso a paso con distintos niveles de granularidad.  
b) Paradigma estructurado.  
c) Paradigma orientado a objetos.  
<p><em><strong>Lenguajes procedurales (estructurados):</strong></em> C, Pascal, COBOL (se usa en Santander, BANAMEX y otros bancos), etc.</p>    
<p><em><strong>Lenguajes declarativos:</strong></em> Se le dice lo que tiene que hacer, pero no el cómo. (SQL, etc.)</p>    
<p><em><strong>Lenguajes funcionales:</strong></em> LISP, Haskell, Clojure, Elixir, etc.</p>  
<p><em><strong>Funciones:</strong></em> Pueden ser puras (tiene argumentos, entre otras cosas) e impuras (no tiene argumentos, entre otras cosas).</p>  
<hr>
<hr>
<h3>Notas</h3>
<p><em><strong>Type:</strong></em> con type se puede ver el tipo de dato en Python.</p>  
<p><em><strong>Type hints:</strong></em> son anotaciones que se ponen en el código, al lado de las variables para 
que el programador sepa qué tipo de datos es el que se espera para esa variable. Hace el código más claro para los que no 
escribieron el programa.</p> 
<p><em><strong>“Azúcar sintáctico”:</strong></em> este término, en inglés <em>syntactic sugar</em>, se usa para referirse a las
expresiones de algún lenguaje de programación que solamente aportan legibilidad al código (hacen que el código
sea más claro).</p>  
<p><em><strong>“Operador morsa”:</strong></em> este operador permite la asignación de valores a una variable en una
expresión. Esto quiere decir que nos permite asignar un valor y devolverlo en la misma expresión, lo que provoca una reducción en
las líneas de código.</p>    
<p><em><strong>Set:</strong></em> el “set” ordena y elimina los números repetidos en un conjunto</p>   
<p><em><strong>*Métodos mágicos:</strong></em> son métodos que definen la manera de comportarse de los objetos en Python 
cuando se hacen operaciones comunes sobre ellos.</p>  
<p><em><strong>Decorador:</strong></em> el decorador (decorator) es una función que modifica otra función</p>  
<p>Una función que no retorna nada en Python, retorna un “none”.</p>  
<hr>
<hr>
<em><strong>Listas:</strong></em>
<p>a) Las listas son estructuras de datos que permiten almacenar gran cantidad de valores.</p>
<p>b) Su equivalente en otros lenguajes son los <em>array</em>.</p> 
<p>c) Las listas también se conocen como colecciones.</p>  
<p>d) En Python, las listas pueden guardar diferen tipo de valores (esto no es posible en otros lenguajes de programación).</p>  
<p>e) Se pueden expandir de manera dinámica, añadiéndose nuevos elementos (esto tampoco es posible en otros lenguajes).</p>
<p>f) Su sintaxis es: <strong>nombre_lista=[elemento1, elemento2, elemento3, elemento4,...]</strong>.</p> 

<em><strong>Tuplas:</strong></em>
<p>a) La tupla es inmutable.</p>  
<p>b) Las tuplas se pueden definir como listas que no permiten añadir, mover o eliminar elementos.</p>  
<p>c) Las tuplas <u>sí permiten extraer porciones</u>, pero el resultado de esta extracción será otra tupla nueva.</p>  
<p>d) Estas estructuras son más rápidas en la ejecución del programa y ocupan menos espacio en memoria.</p>  
<p>e) Su sintaxis es: <strong>nombre_tupla=(elemento1, elemento2, elemento3, elemento4,...)</strong>.</p>  

<em><strong>Diccionarios:</strong></em>
<p>a) Son estructuras de datos que nos permiten almacenar valores de diferente tipo (enteros, decimales, cadenas de
texto) e inclusive listas y otros diccionarios.</p>  
<p>b) La principal característica de estas estructuras es que los datos se almacenan asociados a una clave, por lo 
que se crea una <u>asociación de tipo <em>clave:valor</em></u> para cada elemento almacenado.</p> 
<p>c) Los elementos del diccionario no están ordenados. El ordenamiento no es importante a la hora de 
guardar datos en un diccionario.</p>
<p>d) Su sintaxis es: <strong>nombre_diccionario={elemento1, elemento2, elemento3, elemento4,...}</strong>.</p> 
<h3>Códigos</h3>
<p><strong>1</strong></p>
<code>miLista=["Helios","Gloria","Alfonso","Isabel"]  #Se declara e inicializa la lista.
print(miLista[:]) #Los dos puntos son para que imprima todos los elementos de la lista.</code>  
<p><strong>2</strong></p>
<code>miLista=["Helios","Gloria","Alfonso","Isabel"]  #Se declara e inicializa la lista.
print(miLista[2]) #Imprime Alfonso debido a que es el elemento con índice 2</code>
<p><strong>3</strong></p>
<code>miLista=["Helios","Gloria","Alfonso","Isabel"]  #Se declara e inicializa la lista.
print(miLista[-2]) #Imprime Alfonso, pero en este caso Python le "da la vuelta a la lista"
                   #Se puede decir que cuenta desde el final.</code>
<p><strong>4</strong></p>
<code>miLista=["Helios","Gloria","Alfonso","Isabel"]  #Se declara e inicializa la lista.
print(miLista[0:3]) #Imprime desde Helios hasta alfonso (índice 0 hasta el índice 2)</code>
<p><strong>5</strong></p>
<code>miLista=["Helios","Gloria","Alfonso","Isabel"]  #Se declara e inicializa la lista.
miLista.append("José") #append agrega un elemento
print(miLista[:])</code>
<p><strong>6</strong></p>
<code>miLista=["Helios","Gloria","Alfonso","Isabel"]  #Se declara e inicializa la lista.
miLista.insert(2,"David") #insert agrega el elemento en el índice 2, desplazando a los otros
print(miLista[:])</code>
<p><strong>7</strong></p>
<code>miLista=["Helios","Gloria","Alfonso","Isabel"]  #Se declara e inicializa la lista.
miLista.extend(["David","Israel"]) #extend agrega otra lista a la primera lista
print(miLista[:])</code>
<p><strong>8</strong></p>
<code>miLista=["Helios","Gloria","Alfonso","Isabel"]  #Se declara e inicializa la lista.
print(miLista.index("Gloria")) #Imprime el índice del elemento. Si hay elementos iguales,
                               #entonces siempre da el índice del primero </code>
<p><strong>9</strong></p>
<code>miLista=["Helios","Gloria","Alfonso","Isabel"]  #Se declara e inicializa la lista.
print("Isabel" in miLista) #Devuelve "True" si el elemento está en la lista. Si no, da "False".</code>
<p><strong>10</strong></p>
<code>miLista=[25.67,"Perla",5,"Gloria",False,"Isabel", True] #Las listas pueden contener tipos diferentes
print(miLista[:])</code>
<p><strong>11</strong></p>
<code>miLista=[25.67,"Perla",5,"Gloria",False,"Isabel", True] #Las listas pueden contener tipos diferentes
miLista.pop() #pop elimina el último elemento de la lista (en este ejemplo, "True")
print(miLista[:])</code>
<p><strong>12</strong></p>
<code>miLista=[25.67,"Perla",5,"Gloria",False,"Isabel", True] #Las listas pueden contener tipos diferentes
miLista.reverse() #Invierte los elementos de la lista. El primero será el último.
print(miLista[:])</code>
<p><strong>13</strong></p>
<code>miLista=[25.67,"Perla",5,"Gloria",False,"Isabel", True]*4 #La lista se imprime 4 veces
print(miLista[:])</code>
<p><strong>14</strong></p>
<code>miLista_1=[25.67,"Perla",5,"Gloria",False,"Isabel", True]
miLista_2=[45,"Fabiola",3.1415927]
miLista_3=miLista_1+miLista_2 #El signo de suma concatena las listas (las une)
print(miLista_3[:])</code>
<p><strong>15</strong></p>
![CodigoWalter1](https://github.com/HeliosAlcaraz/Tercer_Semestre_Apuntes_PrimeraParcial/assets/113320901/e973ec4a-141f-4078-aaac-5af6620f809e)
<p><strong>16</strong></p>
![CodigoWalter2](https://github.com/HeliosAlcaraz/Tercer_Semestre_Apuntes_PrimeraParcial/assets/113320901/ffc46294-a183-455d-b552-24bb2230975d)
<p><strong>17</strong></p>
![CodigoWalter3](https://github.com/HeliosAlcaraz/Tercer_Semestre_Apuntes_PrimeraParcial/assets/113320901/3fd825da-a0bd-41b0-a1ed-2db288bd0b44)
<p><strong>18</strong></p>
![CodigoWalter4](https://github.com/HeliosAlcaraz/Tercer_Semestre_Apuntes_PrimeraParcial/assets/113320901/b5ae3192-f017-4fdf-85fc-10ac3946f320)
<p><strong>19</strong></p>
![CodigoWalter5](https://github.com/HeliosAlcaraz/Tercer_Semestre_Apuntes_PrimeraParcial/assets/113320901/c8120474-61fc-4a46-993f-601c917d9fe7)  
<p><strong>20 (Streamlit)</strong></p>
![WalterStreamlit](https://github.com/HeliosAlcaraz/Tercer_Semestre_Apuntes_PrimeraParcial/assets/113320901/2aa453bd-1045-4b7e-a499-f8975821f30a)  
<p>Para correr el código de streamlit (para que salga lo programado como página web) se usa el comando <strong>streamlit run</strong><em> nombre_de_archivo.py</em></p>  
