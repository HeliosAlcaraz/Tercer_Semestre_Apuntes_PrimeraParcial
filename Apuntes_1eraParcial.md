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


