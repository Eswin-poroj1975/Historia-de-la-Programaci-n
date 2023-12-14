# Historia de la Programacion 
Antes de hablar de lenguajes de programación, pensemos en **qué es un lenguaje**. Un lenguaje lo usamos entre humanos para comunicarnos, expresar nuestros sentimientos, o incluso de forma colaborativa para llegar a un fin. Un **lenguaje natural** se define como el **estilo y modo de hablar y escribir de cada persona en particular.**

Ahora, nosotros usamos un **lenguaje de programación** para comunicarnos con una computadora y darle instrucciones, cómo ejecutarlas, a través de qué recursos, etc. Algunos lenguajes permiten ser muy específicos con las instrucciones. En general, un lenguaje de programación es **un formalismo artificial en el cual los algoritmos pueden ser expresados**.

## Niveles de descripción de un lenguaje

Tanto el lenguaje natural como los lenguajes de programación tienen 3 niveles de descripción. Los lenguajes de programación tienen un cuarto nivel, del cual hablaremos más en detalle. Estos niveles de descripción son:

### Gramática/sintaxis

Responde a **¿Qué oraciones son las correctas?** Analiza como están estructuradas las oraciones, palabras/tokens, para que el intérprete (humano o máquina) las pueda entender correctamente. Permite formar frases propias del lenguaje (la gramática/sintaxis no es igual en el Español, el Inglés, o en Python).

### Semántica

Responde a **¿Qué significa una oración correcta?** Indica que es lo que queremos hacer con esa oración. En programación son los ciclos, las variables, etc. Una vez que hemos comprobado que está correctamente escrita, vemos si lo que está escrito es una operación correcta. Por ejemplo: no podemos dividir dos frases, pero si podemos unirlas.

### Pragmática

Responde al **¿Cómo utilizamos una oración significativa?** Una oración significativa es aquella que tiene un significado interpretable. Debemos ser cuidadosos con la pragmática, especialmente en la programación. Las instrucciones que le damos a una computadora no pueden ser tan ambiguas como las que podríamos dar en lenguaje natural.

![Ejemplo de pragmática](https://static.platzi.com/media/articlases/Images/2022-04-23%20%2825%29.png)

### Implementación

Es un nivel de descripción exclusivo de los lenguajes de programación. Se trata de la forma en que se transforman instrucciones en acciones, específicamente mediante el código que escribimos.

## Resumen

Viendo los 4 niveles de descripción como una receta de cocina, la **sintaxis** serían las frases correctas para expresar la receta, la **semántica** se refiere a qué es una receta en particular, la **pragmática** es cómo un chef interpreta la receta, y la **implementación** es la forma en que la receta utiliza los ingredientes.
#estudio_platzi #historia_programacion

>Un paradigma de programación, es la forma en que clasificamos un lenguaje por sus caracteristicas o un estilo de programacion basado en la forma en que aborda un programa y/o las herramientas que utiliza para resolver un problema

Existe una gran cantidad de paradigmas. Sin embargo, todos derivan de 3 paradigmas principales: **imperativo**, **declarativo** y **dirigido por eventos** (este último se verá en una próxima clase).

---
# Cuales son los principales paradigmas de programación
## Programación imperativa

Se trata de expresar cómo debe solucionarse un problema paso a paso. Es el paradigma más utilizado. Se encuentra en lenguajes como Fortran, Java, C, Python, Ruby, etc. De él se derivan paradigmas como la **programación orientada a objetos** o **procedimental**.  
![Programación imperativa en C](https://static.platzi.com/media/articlases/Images/2022-04-24.png)

## Programación declarativa

La programación declarativa consiste en expresar qué problema debe solucionarse, sin especificar cómo hacerlo. Se enfoca en el resultado, y en reducir o evitar los efectos colaterales. Algunos lenguajes en este paradigma son LISP, Haskell, Prolog, SQL, Elixir, XPath, etc. De la programación reactiva se derivan paradigmas como el **funcional**, el **lógico**, **reactivo** o **matemático**.  
![Programación en Haskell declarativa](https://static.platzi.com/media/articlases/Images/2022-04-24%20%281%29.png)

--- 
![[Pasted image 20231205221928.png]]
 > Woh, no sabía cómo funcionaba Haskell jaja, algo curioso y MindBlow es que CSS es un lenguaje declarativo también porque se enfoca en el resultado, de hecho CSS es un lenguaje de query’s porque usas selectores.  
 > 
 > Y si hablamos de query’s y lenguajes declarativos, también está SQL, ya que se enfoca en qué es lo que quieres obtener, no en cómo lo vas a obtener.
 > 
 > Jajaja es simple, a un lenguaje declarativo solo le dices qué quieres hacer, por ejemplo, con CSS tú le dices: “Seleccioname este elemento y ponle estos estilos”, y CSS lo hará, ¿cómo lo hará? Eso no importa porque es un lenguaje declarativo 😄

---
# Máquina abstracta: flujo de datos en computadoras digitales conceptuales
Una **máquina abstracta** es una computadora digital que ejecuta **algoritmos**, los cuales están formalizados para que la máquina entienda. Se trata de una máquina abstracta porque estamos aislando las características de una computadora para llevarlas a este concepto.

## Estructura de una máquina abstracta

La estructura general de una máquina abstracta consiste en:

- Una memoria donde almacena datos y sus programas.
- Un intérprete del lenguaje de programación que maneja las secuencias de control del programa, controla la transferencia de datos y además maneja su memoria.
- Unas operaciones que nos darán un resultado que será la instrucción que deseamos.  
    ![Estructura de una máquina abstracta](https://static.platzi.com/media/articlases/Images/2022-04-23%20%2823%29.png)

### Operaciones de una máquina abstracta

Una máquina abstracta puede realizar operaciones para:

- **Procesar datos primitivos**: Un dato primitivo es aquel con el que un lenguaje de programación trabaja de forma nativa. Puede tener datos primitivos de tipo entero, flotante, booleanos, etc. Ojo, los datos primitivos de un lenguaje, no son necesariamente primitivos en otro.
- **Controlar secuencia de ejecución de operaciones**: La máquina abstracta no solo será capaz de llevar la secuencia de operaciones, también estructuras de control y condicionales como `If`, `Else`. Podrá usar ciclos como `While`, `For`, etc.
- **Controla transferencia de datos**: Esto quiere decir que la información puede pasar de las instrucciones a una estructura de dato y viceversa. Con tal de que la información pueda ser utilizada para sus procesamientos.
- **Manejo de memoria**: La máquina abstracta usa este recurso para almacenar los datos que se derivan de las operaciones de los programas o incluso, almacenar información que le indiquemos.

## Ciclo de ejecución

El ciclo de ejecución se refiere a **los pasos que toma una máquina abstracta para ejecutar operaciones**.

1. Inicia el programa.
2. Se traen las instrucciones a través del intérprete del lenguaje de programación, el cual decodifica las instrucciones.
3. Trae sus operandos para realizar las operaciones.
4. Elige que operación va a ejecutar según las instrucciones.
5. Ejecuta las operaciones indicadas. Una o varias. Incluso la instrucción detener el programa.
6. Si se ejecuta detener, el programa se termina. En caso contrario, se guardan los resultados y se regresa al segundo paso.

![Ciclo de ejecución de una máquina abstracta](https://static.platzi.com/media/articlases/Images/2022-04-23%20%2824%29.png)

### Máquina de Turing:

Es un ejemplo de máquina abstracta. La **Máquina de Turing** tiene 2 cintas en cada lado, y en el centro tiene un dispositivo lector-escritor, es capaz de leer o escribir sobre él mismo. En los rodillos hay instrucciones, indicadas con números 1 y 0. Puede indicar que escriba, lea, etc. En un sentido abstracto, podemos entender que la maquina de Turing realiza los procesos que vimos antes.

## Conclusión

La **máquina abstracta** es un concepto que nos ayuda a entender como funcionan las computadoras y los lenguajes de programación en general. Una **máquina abstracta** es capaz de realizar operaciones complejas si la equipamos para ello.

---
# Programación dirigida por eventos
La **programación dirigida por eventos** se caracteriza por no controlar la secuencia de ejecuciones. Más bien, en la **programación dirigida por eventos** se reacciona a los sucesos ocurridos. Para ello, generalmente los programas corren indefinidamente integrando manejadores de eventos (**event handlers**).

## Eventos y event handler

Los programas dirigidos a eventos se mantienen en estado de reposo, hasta que una acción dispara un **event handler**. Este se encarga de procesar el evento en cuestión. Algunos eventos comunes son:

- Clics (ya sea en un mouse, teclado, pantalla, etc.)
- Sensores (de temperatura, movimiento, etc.)
- Mensajes
- Triggers
- Casos de aplicación
- Solicitudes HTTP

## Casos de uso

Entre los casos de uso de la programación dirigida a eventos encontramos.

- GUIs
- Aplicaciones web
- Sistemas de booking
- Sistemas de alarmas
- Robótica
- Videojuegos

## Funcionamiento

En la programación imperativa tenemos una secuencia de pasos que se van a ejecutar de manera secuencial, y después puede repetirse el ciclo o puede llegar a detenerse el programa porque así lo decidimos o porque forzamos su detención.

Por otro lado, en la **programación dirigida por eventos**, tenemos un **ciclo** el cual mientras haya una condición que sea verdadera, se puede estar ejecutando de manera indefinida. Este ciclo va a escuchar ciertos eventos que van a modificar algunas variables de estado (por ejemplo, el contador de vidas en un videojuego). La modificación de estas variables puede resultar en que el ciclo se detenga, y que el programa finalice.

## Lenguajes y ejemplos

Algunos lenguajes que implementan este paradigma son:

- Java
- JavaScript
- C#
- Librerías/Frameworks de GUI
    - JavaFX, React.js, PyQT
- Prácticamente, cualquier lenguaje orientado a objetos.

Aquí vemos un ejemplo en JavaScript. Nota el uso de **addEventListener**  
![Ejemplo en JavaScript](https://static.platzi.com/media/articlases/Images/2022-04-26%20%283%29.png)

Y un ejemplo en Java. Añadimos un event listener con **addMouseListener**

![Ejemplo en Java](https://static.platzi.com/media/articlases/Images/2022-04-26%20%284%29.png)

## Conclusión

La programación dirigida por eventos nos permite tener programas que corran indefinidamente, y que respondan cuando ocurre un evento. Deja en los comentarios si consideras que la programación orientada a eventos es un paradigma imperativo o declarativo 😉.

---
# Programación Estructurada
La **programación estructurada** apareció como solución a la programación con escritura secuencial, la cual era muy difícil y costosa de leer, mantener y modificar. La **programación estructurada** nace con la **arquitectura de Von Neuman**, la cual reconoce que tanto los programas como los datos que estos arrojan pueden guardarse en memoria.

![Arquitectura de Von Neumann](https://static.platzi.com/media/articlases/Images/2022-04-24%20%282%29.png)

A partir de la arquitectura de Von Neumann se crean las **estructuras de control**, que son la base de la programación estructurada. Con la aparición de las estructuras de control se redujo la necesidad de usar la expresión **“GOTO”**, que se refiere a llamar una línea de código cualquiera desde otra línea de código. A continuación vemos un ejemplo de un diagrama de flujo estructurado que implementa la [serie de Fibonacci](https://platzi.com/clases/2397-python-profesional/39532-la-sucesion-de-fibonacci/).  
![Fibonacci](https://static.platzi.com/media/articlases/Images/2022-04-24%20%283%29.png)

Algunos de los primeros lenguajes que implementaron la programación estructurada son FORTRAN, Pascal, COBOL, ADA, Perl y C.

## Características de la programación estructurada

La programación estructurada se caracteriza por el uso de estructuras de control (condicionales y ciclos). Otras características de la programación estructurada (y de los lenguajes imperativos en general) son:

- Uso de entradas/salidas (input y output, o **I/O**)
- Manejo de **errores y excepciones**.
- Abstracción de procedimientos.
- Expresiones y asignación.
- Soporte para estructuras de datos.

---
## Código de Fibonacci
```C++
#include <iostream>
using namespace std;

int main(){
	int n, fib0 = 0, fib1 = 1, c, i;
	
	cout << "Interacion de Fibonacchi" << endl;
	cout << "Ingrese el numero n" << endl;
	cin >> n;
	
	for(i=1; i<=n; i++){
		cout << fib0 << " ";
		c = fib0 + fib1;
		fib0 = fib1;
		fib1 = c;
	}
	return 0;
}
```

---
# Programación Funcional

>Woow, todo esto fue lo que me preguntaron en mi primera entrevista técnica para ser software engineer en México. Fue tipo así  
-Qué es una clase?  
Es la definicón de un objeto 😃  
-y qué es un objeto?  
Es una instancia de una clase, es como si una clase fuera un cortador de galleta y el objeto es una galleta  
-y qué es una instancia?  
Los objetos se almacenan en memoria y la instancia es el espacio que hace referencia a ellos  
-muy bien, ahora cuentame qué es el polimorfismo?  
-…  
-no te preocupes, dime qué es el encapsulamiento?  
-el encapsulamiento permite limitar ? los métodos de un objeto?  
-ok… y qué es lamnda?  
-…una letra griega :v  
Estudie informatica y me sentia super confiada, la verdad con estas clases y las entrevistas ténicas me doy cuenta del gap mental que tenia entre cada concepto.

---

La programación funcional es un paradigma declarativo que usa **funciones** como “**ciudadanas de primera clase**”. Las funciones (en programación) son fragmentos de código reutilizables, que pueden recibir datos y dar salidas a otros datos como resultado, incluyendo otras funciones. Mediante la programación funcional se busca eliminar o reducir los **efectos secundarios**.

En la programación funcional se pueden crear **funciones de orden superior (HOF)**. Prioriza el uso de **recursividad** y **HOF** para resolver problemas.

## Origen de la programación funcional

En los años 30, Alonzo Church desarrolló el cálculo **Lambda**. Alan Turing demostró que este es equivalente a las máquinas de Turing. A finales de los 50, se desarrolló **LISP**, implementando la notación **lambda** de Church. Aquí un ejemplo en LISP de cómo se ve un _“hola mundo”_ y una función recursiva (que se llama a sí misma) donde se calcula el [factorial](https://platzi.com/clases/2884-notacion-matematica/47332-sumatoria-y-factorial/) de un número `n`.

```lisp
(print "Hello, World!")
(defun factorial (n)
    (if (= n 0) 1
        (* n (factorial (- n 1)))))
```

## Funciones

En matemáticas, una función se define como una relación entre dos conjuntos que asigna cada elemento del primero, un elemento del segundo o ninguno.  
Por ejemplo, una función que toma un valor “X” y genera un valor “Y”.

```
f(X) = X + 3
f(X) = X^2 + 3
```

Un ejemplo de funciones en Python es el siguiente. La función suma recibe dos números (a y b) y retorna la suma de los dos números. Aquí podemos ver que el concepto de función en matemáticas y en programación es parecido.

```python
def suma (a, b):
    return a + b
operacion_1 = suma(3, 2)
```

Las funciones también pueden hacer uso de otras funciones, como en el siguiente ejemplo.

```python
def es_par(x):
    return not es_impar(x)
```

Es más, las funciones pueden llamarse a sí mismas (recursión)

```python
def fibonacci(n):
    if n<=1:
        return m
    else:
        return fibonacci(n-1)+fibonacci(n-2)
```

## Conceptos de la programación funcional

Al principio mencionamos conceptos como **“ciudadanas de primera clase”**, **funciones de orden superior** y **efectos secundarios**. Definamos estos (y más) conceptos.

### Funciones como ciudadanas de primera clase

El que las funciones sean **ciudadanas de primera clase** implica que son reconocidas como un tipo de dato más. Esto hace que se puedan usar en cualquier parte del programa.

### Funciones de orden superior

Una función de orden superior puede recibir una o varias funciones como parámetro. Además, puede retornar otra función.

### Funciones puras

Una función es pura si cumple con los siguientes requisitos.

- **Es determinista**: para un parámetro, la función siempre va a retornar el mismo resultado siempre y cuando no se cambie dicho parámetro (por ejemplo, una función que retorne un valor aleatorio no es determinista).
- Un valor de entrada da un solo valor de salida.
- No genera efectos secundarios.
- No incluye funciones impuras.

### Funciones lambda

Una función **lambda** es una función anónima, es decir, que no se le asigna un nombre. Normalmente, se usan en una única sección del código. Por lo general realizan operaciones simples.

Un ejemplo de una función lambda que multiplica dos números en Python:

```python
x = lambda a, b: a**b
print(x(3,3))
```

### Efectos secundarios (side effects)

Es común escuchar de **efectos secundarios** cuando hablamos de programación imperativa. Lo podemos ver cuando manejamos funciones o variables de contexto global o que están delimitadas. Cuando escribimos código sabemos que lo que está dentro de una función, no afecta a otra, si es que usamos la sintaxis correcta. Pero también existen funciones que usan parámetros o que tienen alcance global y pueden tener efectos secundarios.

Los efectos secundarios son cambios observables en partes de un programa como:

- El estado de la aplicación.
- Valores de datos.
- Modificación de archivos.

## Lenguajes y ejemplos

Este es un ejemplo en Haskell, donde calculamos el factorial de un número. En ejemplos anteriores habíamos podido ver como se define el tipo de dato, después se asignan los tipos de valores y se empieza a llamar a la función. Podemos ver que el código no es tan amplio como si lo hubiéramos escrito de forma no recursiva con otros lenguajes.

```haskell
module Main where

import Text.Printf

factorial :: Integer -> Integer
factorial 0 = 1
factorial n = n factorial (n - 1)

line x = printf "%d! = %d\n" x $
factorial x

main = mapM_ line [0..16]
```

Aquí otro ejemplo con **F#**, donde vemos que también es recursivo porque la función factorial se llama a sí misma.

```haskell
let rec factorial n = 
    match n with
    | 0 | 1 -> 1
    | _ -> n * factorial(n-1)
```

Otros lenguajes funcionales son SCHEME, CLOJURE, RACKET y ERLANG.

## Conclusión

La programación funcional nos permite escribir código especificando qué queremos hacer más que cómo se debe hacer. A su vez, nos permite evitar efectos secundarios. Es importante entender conceptos como **funciones de orden superior**, **recursividad** o **funciones puras** para poder hacer un buen uso de la programación funcional.

---
# Programación Lógica
La programación lógica **es un paradigma declarativo que expresa los objetivos como una colección de afirmaciones o reglas acerca de los resultados y restricciones en lógica matemática**. Entre sus áreas de aplicación encontramos el NLP (Procesamiento de lenguaje natural), la recuperación de información en bases de datos y aplicaciones matemáticas.

## Cláusulas de Horn

La programación lógica se basa en las **Cláusulas de Horn**. Estas son preposiciones definidas por predicados, donde tenemos un **hecho** (algo que damos por sentado) y tenemos uno o varios predicados. Lo correcto sería tener por lo menos 2, para poder determinar si algo es verdadero o falso, también se les conoce como cuerpo/body. Las cláusulas de Horn están relacionadas con las [tablas de verdad](https://www.youtube.com/watch?v=Pfyuv5ZnNNw).  
![Cláusula de horn](https://static.platzi.com/media/user_upload/1-9eec6a3e-8472-4216-b214-02e4be6bd1a0.jpg)

H= Hecho/Head of the rule.  
P= Predicado/Body

### Ejemplo de cláusula de Horn

Podemos decir que es verdadero que está nevando en la ciudad, C es el nombre de la ciudad. Si está lloviendo y hace frío, entonces es verdadero que está nevando. Y, por el contrario, si quisiéramos negar que está lloviendo, pero hace frío, entonces es falso que está nevando. Esto tiene una estrecha relación con las tablas de verdad.

```prolog
nevando(C) ← lluvia(C), frío(C)
```

## Origen de la programación lógica

La programación lógica viene de los años 60, cuando Cordell Green propuso el uso de cláusulas en programas a finales de los 60. El lenguaje **Prolog** impulsó este paradigma. Otros lenguajes lógicos son Alf, Fril ,Mercury, Oz ,Visual Prolog y XSB.

No es muy frecuente el uso de programación lógica en la industria. Se usa más en investigación y ámbitos académicos.

### Ejemplos de Prolog

Este es un ejemplo de _“hola mundo”_ en Prolog. Nótese que al final se imprime **true**.

```prolog
% Hola mundo

?- write('Hello World!'), nl
> Hello World!
> true
```

En el siguiente ejemplo vemos como le indicamos que hay personas que hablan un lenguaje, hacemos la evaluación de la persona 1 con la persona 2 y cuál es el resultado. Luego hacemos también la evaluación, preguntando “Quién habla francés” El resultado retornado debería ser “Juan”.

```prolog
speaks(juan, french)
speaks(isabel, english)
speaks(eduadro, french)
speaks(eduardo, english)

talkswith(Person1, Person2) :-
speaks(Person1, L),
speaks(Person2, L),
Person1 \= Person2

?- speaks(Who, French)
```

## Conclusión

La programación lógica es un paradigma utilizado sobre todo en entornos académicos. Se basa en el uso de Cláusulas de Horn, y tiene una relación estrecha con las tablas de verdad.

>💡 La **programación lógica** permite resolver problemas mediante **predicados**, este es usado en la **Inteligencia Artificial**.

---
# Programación Orientada a Objetos (POO)
La programación **orientada a objetos (POO)** se basa en el concepto de **objeto**. Un objeto es una abstracción de una entidad que posee datos en forma de **propiedades o atributos**, y procedimientos en forma de **métodos**. Por ejemplo, si vemos a un humano como un objeto, un humano tiene **propiedades** como su altura o color de cabello, así como **métodos** como leer, escribir, comer, etc.

El primer lenguaje orientado a objetos fue **Simula**. Otros lenguajes orientados a objetos son C++, C#, PHP, Ruby, Python, etc.

## Conceptos principales de la POO

Ya hablamos del concepto de **objeto**. Ahora introducimos otros conceptos fundamentales dentro de la programación orientada a objetos.

### Clases

Una **clase** es un molde o fábrica de objetos. En una clase se **definen** las propiedades y métodos que pueden tener un objeto. Se dice que **un objeto es una instancia de una clase**. Cuando se crea un objeto a partir de una clase, se definen los valores de las propiedades del objeto.

### Propiedades

Las propiedades son características que distinguen un tipo de objeto de otro, pero que varían entre objetos. Por ejemplo, los objetos de tipo humano pueden tener distintos colores de cabello, pero la propiedad “color de cabello” es una que existe en todos los humanos ~~(en los calvos esta propiedad valdría null)~~.

### Métodos

Los métodos son acciones o procedimientos que puede llevar a cabo un objeto. Por ejemplo, si un profesor fuera un objeto, un método del profesor sería “dar clase”.

## Pilares de la POO

La programación orientada a objetos se fundamenta en 4 pilares. Es importante entender estos pilares, ya que la POO es el paradigma más utilizado dentro del desarrollo de software.

### Abstracción

La abstracción se refiere a aislar las características de un objeto. Se trata de conceptualizar objetos y cuáles son sus características

### Herencia

La herencia permite que una clase **herede** propiedades y métodos de otra clase. Por ejemplo, la clase _“perro”_ hereda de la clase _“animal”_. En este caso diríamos que la clase _“perro”_ es hija de la clase _“animal”_.

### Encapsulamiento

El encapsulamiento ayuda a aislar parte del código de una instancia. Esto permite que cuando sea llamada no altere su estado por accidente o por efecto colateral de los métodos o comportamientos de otros objetos con los que puede interactuar.

### Polimorfismo

El [polimorfismo](https://platzi.com/clases/2034-php-poo/32133-polimorfismo/) significa que ante los mensajes o llamados que reciba una clase o una instancia los va a interpretar de una forma distinta a como lo harían clases o instancias distintas.

## Ventajas y desventajas de la POO

Como cualquier paradigma de programación, la POO presenta varios pros y contras.

### Ventajas

- Código reutilizable.
- Reducción de redundancia.
- Fácil de mantener.
- Seguridad (mediante métodos, propiedades y clases privadas/protegidas).

### Desventajas

- Tamaño (cuando una clase es muy general y tiene muchas clases hijas)
- Esfuerzo (por la especificidad que requieren)
- Velocidad del desarrollo (por el esfuerzo)

## Conclusión

La programación orientada a objetos es el paradigma más utilizado gracias a que permite reutilizar el código de una manera segura y fácil. Es fundamental entender los conceptos y pilares de la programación orientada a objetos.

---
# Programación por Procedimientos
La **programación procedural** o **procedimental** se deriva de la **programación estructurada**. Consiste en dividir el código en secciones lógicas llamadas rutinas o **procedimientos**, donde cada procedimiento resuelve una tarea específica, y se ejecuta cada vez que sea necesario. Cabe destacar que un procedimiento puede llamar a otros procedimientos. Algunos de los primeros lenguajes procedurales son FORTRAN, ALGOL, COBOL Y BASIC.

![Flujo de un programa procedural](https://static.platzi.com/media/articlases/Images/2022-04-24%20%284%29.png)

## Comparación con la programación orientada a objetos

Hay algunas similitudes entre la **programación procedural** y la **orientada a objetos** (tema de la siguiente clase).

![Comparación entre procedural y POO](https://static.platzi.com/media/articlases/Images/2022-04-24%20%286%29.png)

---
# Paradigmas de la Programación
Un **paradigma** es una teoría o conjunto de teorías cuyo núcleo central se acepta sin cuestionar y que suministra la base y modelo para resolver problemas y avanzar en conocimiento.

## Paradigmas en programación
En programación, cuando hablamos de paradigmas, podemos hablar de **cómo se clasifican los lenguajes basados en sus características**. También podemos referirnos a **estilos de programación**, es decir, a cómo se aborda un problema o qué herramientas se utilizan. 

> **En general, que un lenguaje tenga un paradigma específico significa que limita o prohíbe ciertas acciones.**

### Paradigmas y lenguajes de programación

Podemos clasificar los lenguajes de programación en función de su paradigma.

**Paradigmas puros**: lenguajes como Smalltalk que es **POO** o Haskell que solo es **funcional**  
**Multiparadigma**: lenguajes como Python, Ruby, Scala, PHP, etc.

### Discusión

Cabe preguntarnos, ¿es correcto etiquetar así a los lenguajes, o el estilo de programación de alguien? ¿Cómo afectan los paradigmas a los modelos de programación y patrones de diseño?

---
 > Un **paradigma de programación** es una forma o estilo de **programación de software**.

---
# Programación Concurrente
Imagina que trabajas en una panadería. Mientras se calienta el horno, estás cortando masa, preparando panes, y una vez que se hornean, al sacarlos hay que esperar a que se enfríen y después colocar una cobertura de chocolate. Tú intentarás optimizar los recursos. Mientras el horno se está calentando, debes preparar más masa, para que así, cuando termine, inmediatamente metes el otro lote de masa.

También puedes contratar a una persona que te ayude. Divides las tareas, ejecutando el **paralelismo**, que es dividir las tareas entre los recursos disponibles (siempre y cuando puedan dividirse).

## Concurrencia

La **concurrencia** ocurre cuando hay una serie de peticiones a un mismo recurso que puede ser limitado, y se atienden esas peticiones de forma parcial o totalmente desordenada. Una analogía útil para entender puede ser la panadería. Imagina que tu panadería empieza a crecer, porque es bastante concurrida y los clientes empiezan a acumularse.

## Concurrencia vs. paralelismo

En la **concurrencia** tenemos una serie de peticiones con un solo recurso limitado para atenderlas. Cabe preguntarse ¿cuál sería el orden y la prioridad en la que se atienden las peticiones? Por otro lado, en el **paralelismo** tenemos recursos divididos que pueden atender las peticiones al mismo tiempo sin ningún problema. El **paralelismo** y la **concurrencia** son conceptos diferentes, pero que van de la mano.

## Secuencia vs. Concurrencia

En una **secuencia** tenemos los pasos A, B, C, D. Y estos serán atendidos en el orden que se hizo la petición. En cambio, en **concurrencia** podemos iniciar en el proceso A, saltar al D, luego al C, completar el A y después pasar al último proceso. Todo esto se hace mediante los [hilos](https://platzi.com/clases/1441-ruby/15856-concurrencia-vs-paralelismo-threads-en-ruby/) de un **proceso**.

### Estados de un hilo

Un **hilo** tiene 5 estados posibles

- **Creado**: no está listo para correr.
- **Ejecutable/Listo**: espera para ejecutarse.
- **Ejecutando**: se ejecuta en el procesador.
- **Bloqueado**: espera a entrar al código que requiere acceso al recurso compartido o abandona el procesador.
- **Terminado**: se ha detenido y no puede reiniciarse.

### Sección crítica del hilo

Es una sección de código que requiere acceso exclusivo a una variable compartida. Sucede cuando varios hilos deben **“comunicarse entre sí para decidir cuál va a tener acceso al recurso en el momento”**. Esta sección crítica causa distintos problemas al usar concurrencia, los cuales exploraremos en la próxima clase.

---
# Problemas de la Programación Concurrente
La programación concurrente se basa en el uso de **hilos**. Cuando tenemos varios hilos compartiendo recursos entre sí se pueden presentar algunos problemas, entre ellos:

## Carreras (race conditions)

Los **race conditions** ocurren cuando dos o más hilos desean acceder a un recurso lo más pronto posible. Por ejemplo, tenemos una variable C inicializada en 0, pero después en alguna parte del código a C se le asigna el valor de C + 1. Entonces un hilo llegará primero y al ver que vale 0, le agregará el valor de 1, almacena ese dato y ahora C vale 1.

Pero si otro hilo llega después, pensará que C vale 1, entonces añadirá otro 1, almacenará ese dato y entonces C vale 2. Esto puede ser un problema en un sistema automatizado de dosificación de medicamentos. Sí el sistema es concurrente, ¿Entonces que hará? ¿Le dará una dosis o dos dosis? ¿Cómo se resuelve?.

## Puntos muertos (deadlock)

Un **deadlock** ocurre cuando un hilo espera por un evento que nunca sucederá. Para que suceda un **deadlock** deben de cumplirse 4 condiciones:

- Los hilos deben tener acceso exclusivo a los recursos.
- Los hilos deben contener algunos recursos mientras esperan otros.
- Los recursos no se pueden eliminar de los hilos en espera.
- Existe una cadena circular de hilos en las que cada uno contiene uno o más recursos del siguiente hilo.

## Problema de los filósofos

El **problema de los filósofos** plantea que hay una mesa redonda con 5 filósofos conversando. Frente a ellos hay un plato de comida, y hay un palillo chino a la derecha y otro a la izquierda (5 palillos en total). Para comer se necesitan dos palillos chinos, eso significa que no todos podrán comer al mismo tiempo.

Hay muchas formas de abordar el problema, pero esas soluciones pueden dar otros problemas. Podría ser un sistema de turnos, pero entonces algunos se quedarían esperando hasta que la comida esté fría.

## Estrategias para evitar los deadlocks

Dos estrategias para evitar que se cumpla alguna de las condiciones que producen deadlocks son el uso de **semáforos** o **monitores**.

- **Semáforos**: Funcionarían como una variable de tipo entero, asociado a un mecanismo de cola de hilos. Si el semáforo toma valores de “0” y “1”, es binario. En caso contrario, es un “semáforo contador”.
- **Monitores**: Estructuras de datos abstractas basados en los monitores o kernel de los S.O. Los monitores tienen 4 componentes principales:
    - **Inicialización**: contiene código a ser ejecutado.
    - **Datos privados**: procedimientos que se utilizan desde dentro del monitor.
    - **Métodos del monitor**: procedimientos que se pueden llamar desde fuera.
    - **Cola de entrada**: hilos que llaman a algún método del monitor, pero no tienen permiso para ejecutarse aún.

## Algunos lenguajes que implementan concurrencia

Estos lenguajes pueden hacer uso de la concurrencia, aunque de forma distinta entre ellos.

- JavaScript
- C#
- Golang
- Rust
- Elixir
- Haskell

## Conclusión

La programación concurrente nos ayuda a ejecutar procedimientos de manera más eficiente en algunos casos, al no ejecutarlos de manera secuencial. Sin embargo, la programación concurrente trae una serie de problemas como las race conditions y deadlocks, para los cuales hay distintas estrategias que ayudan a evitarlos.

---
# Década de los 40: primeras computadoras y lenguajes ensambladores
Ya que conoces conceptos sobre paradigmas de programación, es buen momento para conocer la historia y cronología de algunos lenguajes de programación, empezando por los años 40.

## Primeras computadoras

La primera computadora no fue una máquina abstracta, eso es un concepto teórico. Sin embargo, sabíamos que las computadoras épocas atrás, tenían tamaños enormes, ocupaban canchas de tenis y trabajaban con switches. Hay distintos criterios para definir cuál fue la primer computadora y algunos autores mencionan que fue la **EDSAC**, que contó con las siguientes características

- Era electrónica y digital.
- Realizaba 4 operaciones básicas.
- Era programable.
- Almacenaba programas y datos.

Las precursoras de la **EDSAC** carecían de herramientas lingüísticas para ser programadas al nivel de la **EDSAC**. Estas iniciaron con **código máquina**, llamados **first-generation languages (1GL)**.

## Lenguajes ensambladores

Los **lenguajes ensambladores** son representaciones simbólicas del lenguaje máquina. Un programa **“ensamblador”** traduce las instrucciones a código máquina. Cada máquina tenía su propio lenguaje, había nula portabilidad. Son llamados **second-generation languages (2GL)**

---
# Década de los 50: Fortran y Algol
En la Década de los 40. Aparecieron los primeros lenguajes para comunicarnos con las máquinas, pero tenían ciertas limitaciones técnicas.

Entonces en los 50 aparecieron los primeros lenguajes de alto nivel (conocidos como trhid generation languages, o 3GL), que se caracterizan por ignorar las limitaciones del hardware y manejar el concepto de portabilidad. A partir de estos lenguajes nacieron otros que veremos en las próximas clases, pero…

## ¿Por qué hay tantos lenguajes de programación?

Hoy en día, a diferencia de los 50, vemos una gran variedad en lenguajes de programación. Y es que hay lenguajes que cumplen distintos propósitos, ya sea:

- Propósitos netamente comerciales
- Aplicaciones específicas
- Nuevas metodologías de trabajo
- Implementaciones como desarrollador
- Usar nuevos paradigmas

Muchos lenguajes más modernos son descendientes de los lenguajes de los 50.

## Lenguajes de programación de los 50

Entre los lenguajes más conocidos desarrollados en esta década encontramos

### Fortran (1957)

Desarrollado por IBM y John Backus, el principal uso de FORTRAN era en trabajos numéricos y científicos, en la máquina IBM 704. Es un lenguaje utilizado (en menor medida) hoy en día. Sus versiones actuales implementan las estructuras de control, funciones, memoria dinámica, comentarios y sub-rutinas. A continuación podemos ver un ejemplo de código en FORTRAN.

>Buenas, como dato les dejo que FORTRAN (que corrijo un pequeño detalle del profe jaja) proviene de FORmula TRANslation - Traducción de Fórmulas y justamente se llamaba así porque se había creado para programación numérica/científica, también para aplicaciones en la física o la ingeniería. Saludos!

![Fortran code](https://static.platzi.com/media/articlases/Images/2022-04-27%20%281%29.png)

### ALGOL (1958-1960)

**ALGOL** es una familia de lenguajes que hace uso de notaciones matemáticas, gramáticas generativas y estructuras de control. Aquí vemos un ejemplo de **ALGOL**.  
![ALGOL ejemplo](https://static.platzi.com/media/articlases/Images/2022-04-27%20%282%29.png)

---
# Década de los 60: LISP, COBOL, Simula
Es natural que después de los 50 se crearan nuevos lenguajes de programación para nuevas máquinas. Entre los lenguajes más destacados de la década de los 60 encontramos:

## LISP (List Processor)

**LISP** fue el primer lenguaje de aplicación no-numérica. Se utilizaba para traducción automática de textos. Hacía uso de **“expresiones S”**. Cabe destacar que LISP introdujo el concepto de programación de orden superior, y podía usar memoria dinámica.

Había distintas variantes de LISP para distintas máquinas (LISP Machines), por lo que no era un lenguaje muy portable. Algunos dialectos comunes de LISP son **Racket**, **Common Lisp**, **Scheme** y **Clojure**.

![Factorial recursivo en LISP](https://static.platzi.com/media/articlases/Images/2022-04-28.png)

## COBOL

**COBOL** es acrónimo de **Common Business Oriented Language**. En un lenguaje imperativo y procedural, (hoy en día) orientado a objetos, y que buscaba acercarse lo más posible al inglés. Cabe destacar que Grace Hopper lideró el equipo que lo revisó y lo volvió un estándar. Un programa de [COBOL](https://platzi.com/cursos/cobol/) se divide en 4 secciones:

- **Procedimiento**: código de aspectos algorítmicos.
- **Datos**: descripción de los datos.
- **Ambiente**: especificación del ambiente externo al programa indicado por la máquina física.
- **Identificación**: datos del programa, autor, etc.

![Multiplicación de 3 números en COBOL](https://static.platzi.com/media/articlases/Images/2022-04-28%20%281%29.png)

## SIMULA

**SIMULA** es un lenguaje descendiente de **ALGOL**. Está diseñado para cálculo de simulaciones de colas. Se destaca por introducir las clases, objetos, sub-tipos y el método dinámico de despacho. Marcó un antes y un después en los paradigmas, y fue predecesor para Smalltalk y C++ (lenguajes orientados a objetos). Se encuentran trabajos hasta el 2000 en este lenguaje. A continuación vemos un “hola mundo” en SIMULA.

![Hola mundo en SIMULA](https://static.platzi.com/media/articlases/Images/2022-04-28%20%282%29%281%29.png)

Aquí vemos la implementación de una clase en SIMULA  
![2022-04-28 (3).png](https://static.platzi.com/media/articlases/Images/2022-04-28%20%283%29.png).

---
# Década de los 70: C, Pascal, Smalltalk, Prolog
Gracias a la llegada de los microprocesadores surgieron nuevos lenguajes de programación que se adaptaron a la nueva arquitectura. Las máquinas se volvieron más pequeñas y veloces. Además, gracias a los microprocesadores, se abrió la posibilidad de la portabilidad (que un mismo lenguaje sirva para distintas máquinas). Entre los lenguajes más destacados de esta década encontramos:

## C

**C** es un lenguaje de programación de propósito general. Originalmente desarrollado por Dennis Ritchie entre 1969 y 1972 en los Laboratorios Bell, tiene su nombre como evolución del anterior lenguaje B (a su vez basado en BCPL). Estaba originalmente pensado para el sistema operativo UNIX.

Se trata de un lenguaje de tipos de datos estáticos, débilmente tipado, de medio nivel. Dispone de las estructuras típicas de los lenguajes de alto nivel, pero también de construcciones del lenguaje que permiten un control a bajo nivel.

Por ser de relativamente bajo nivel y tener un modesto conjunto de características, se pueden desarrollar compiladores de [C](https://platzi.com/cursos/lenguaje-c/) fácilmente. En consecuencia, el lenguaje C está disponible en variedad de plataformas. A continuación un ejemplo en C.

![Factorial en C](https://static.platzi.com/media/articlases/Images/2022-04-28%20%284%29.png)

## Lenguaje Pascal

**Pascal** es un lenguaje de programación creado por el profesor suizo Niklaus Wirth entre los años 1968 y 1969, y publicado en 1970. Su objetivo era crear un lenguaje que facilitara el aprendizaje de programación a sus alumnos, utilizando la programación estructurada y estructuración de datos.

Pascal fue el lenguaje primario de alto nivel utilizado para el desarrollo en el Apple Lisa, y en los primeros años del Macintosh.

Se caracteriza por ser un lenguaje de programación fuertemente tipado, pero que permite la definición de nuevos tipos de datos con el **primitivo type**. Además, introdujo el código intermedio. Es decir, el código Pascal se compila a un formato llamado “**P-code**”, que después es interpretado (similar a como funciona la [Java Virtual Machine](https://platzi.com/clases/2245-kotlin/36586-que-es-la-java-virtual-machine/)). Aquí un ejemplo de cómo calcular el factorial en Pascal.

![Factorial en Pascal](https://static.platzi.com/media/articlases/Images/2022-04-28%20%285%29.png)

## Smalltalk

Los orígenes de **Smalltalk** se encuentran en las investigaciones realizadas por Alan Kay, Dan Ingalls, Ted Kaehler, Adele Goldberg y otros durante los años 70 en el _Palo Alto Research Center_. Es un lenguaje reflexivo de programación, 100% orientado a objetos y con tipado dinámico. Se caracterizó por incluir los objetos de manera primitiva (es decir, no hay que traer paquetes o librerías).

Smalltalk manejó conceptos como las clases, el encapsulamiento, los métodos públicos y las instancias privadas. Además, Smalltalk apuntaba a ser no solo un lenguaje sino un entorno completo de programación. A continuación vemos un ejemplo de cómo se crea una clase en Smalltalk.  
![Clase en Smalltalk](https://static.platzi.com/media/articlases/Images/2022-04-28%20%286%29.png)

## Meta Language (ML)

Diseñado por Robin Milner y su equipo a mitad de los 70, **ML** era utilizado principalmente para manipular información simbólica. Es un lenguaje declarativo y funcional, orientado a la investigación

Al igual que Pascal, es un lenguaje de tipado estático. No obstante, se destacó por ser el primer lenguaje que contó con un sistema de inferencia de tipos. Es decir, no es obligatorio declarar el tipo de dato de una variable. A continuación un ejemplo del algoritmo [insertion sort](https://platzi.com/clases/1775-poo-python/25266-ordenamiento-por-insercion/) en ML.  
![Insertion sort en Meta Languaje](https://static.platzi.com/media/articlases/Images/2022-04-28%20%287%29.png)

## Prolog

**Prolog** es un lenguaje de programación lógica. Ideado a principios de los años 70 en la Universidad de Aix-Marseille I (Marsella, Francia) por Alain Colmerauer y Philippe Roussel, está basado en las **cláusulas de Horn**. Se mantiene vigente a día de hoy, ya que se usa en el campo de la Inteligencia artificial y el procesamiento natural del lenguaje (NLP). Como dato curioso, el primer intérprete de Prolog fue desarrollado en FORTRAN.

He aquí un ejemplo de Prolog (el cual vimos en clases pasadas).

```prolog
speaks(juan, french)
speaks(isabel, english)
speaks(eduadro, french)
speaks(eduardo, english)

talkswith(Person1, Person2) :-
speaks(Person1, L),
speaks(Person2, L),
Person1 \= Person2

?- speaks(Who, French)
```

---
# Década de los 80: Computadoras personales, POO (programación orientada a objetos), C++, Python
En la década de los 80 aparece la computadora personal, eliminando la necesidad de ir a institutos de investigación ni universidades para acceder a una computadora. Por la popularidad de los dispositivos, los lenguajes se empiezan orientar a la interfaz gráfica, cambiando el paradigma. En esta década aparecieron lenguajes destacados como C++ y Python.

## C++

**C++** se creó en 1986 definido por Bjarne Stroustrup como parte de una extensión de C. Se dice que todo programa válido en C es también un programa válido en [C++](https://platzi.com/cursos/c-plus-plus/). Se destacó por incorporar el uso de clases, mejorar el sistema de tipado, implementar templates manipular objetos de forma directa y mejorar el sistema de herencia. Aquí un ejemplo de cómo calcular el factorial en C++.

![Factorial en C++](https://static.platzi.com/media/articlases/Images/2022-04-28%20%288%29.png)

## Python

**Python** es un lenguaje creado Guido van Rossum a finales de los 80. Es interpretado, de alto nivel, multiparadigma y de propósito general. Tiene librerías para procesamiento matemático, asincronismo, inteligencia artificial, análisis de datos, etc. Tiene un gran rango de aplicaciones como el desarrollo web, IoT, móviles, videojuegos, servidores, IA y Ciencia de Datos.

Cabe destacar que [Python](https://platzi.com/cursos/python/) tiene una filosofía de desarrollo conocida como el **Zen de Python**, que busca hacer el código más legible. Los postulados de este zen son:

- Bello es mejor que feo
- Explícito es mejor que implícito
- Simple es mejor que complejo
- Complejo es mejor que complicado
- La legibilidad cuenta

Como es costumbre, aquí te dejo un ejemplo de cómo se calcula el factorial en Python.

![Factorial en Python](https://static.platzi.com/media/articlases/Images/2022-04-28%20%289%29.png)

🐍 **Python** es un **lenguaje de programación** **basado** en **LISP** y **C**.

---
# Década de los 90: Desarrollo web, Java, JavaScript
En los 90 surgieron innovaciones que permitieron la comunicación entre computadoras muy lejanas entre sí: el navegador, el Internet y la web. A partir de estas invenciones surgieron lenguajes enfocados a la web, como Ruby, PHP, **Java** y **JavaScript**. Hablemos más en profundidad sobre estos últimos.

## Java

Desarrollado por el green team dirigido por Jim Goslin en Sun Microsystems en 1990, **Java** es uno de los lenguajes más populares incluso en la actualidad. Su objetivo era ser utilizado en dispositivos de poder limitado conectados en una red.

Después se vio el potencial de Java en la web utilizando “applets”. Estas se caracterizaban por ser seguras y portables (sin embargo, te pedían instalar Java)

Una de las características de [Java](https://platzi.com/cursos/java-basico/) es el uso de la [**_Java Virtual Machine (JVM)_**](https://platzi.com/clases/2245-kotlin/36586-que-es-la-java-virtual-machine/). En Java el código se compila a bytecode, que después es interpretado por la **JVM**. Cabe destacar que la JVM fue incorporada al navegador Netscape en 1995.

### Seguridad, otras características y ejemplos

Java no genera errores de ejecución no detectados. Además, Java realiza la verificación de tipos durante la compilación **Y** la interpretación del bytecode.

Otras características del lenguaje son:

- Simplicidad del lenguaje
- Garbage Collector
- Manejo implícito de punteros
- Uso de hilos para concurrencia

A continuación vemos un “hola mundo” en Java.

```java
// JAVA
// Hola, mundo!
public class HelloWorldApp {
    public static void main(String[] args) {
        System.out.println("Hello World!");
     }
}
```

Además de cómo calcular el factorial en Java.

```java
// JAVA
// Factorial de n
public double factorial (double numero) {
    if (numero == 0)
        return 1;
    else
        return numero * factorial(numero-1);
}
```

## JavaScript

[**JavaScript**](https://platzi.com/cursos/basico-javascript/) es un lenguaje multiparadigma de alto nivel, compilado **“just-in-time”** (se compila a medida que se ejecuta). Es débilmente tipado y dinámico, es decir, no se debe especificar los tipos de las variables, y estos pueden cambiar. Está basado en [prototipos](https://platzi.com/clases/1642-javascript-profesional/22164-prototype/).

Se usa del lado del cliente y del servidor. En 2012 se volvió un estándar y es soportado por todos los navegadores por defecto.

Esto es un “hola mundo” en JavaScript.

```javascript
console.log("hola mundo")
```

Y así se puede calcular el factorial (de 3) en JavaScript

```javascript
function factorial(n) {
    if (n === 0)
        return 1;
    return n * factorial(n - 1);
}
factorial(3);
```

![[Pasted image 20231213185019.png]]

## ¿Por qué se llama JavaScript?
---
Brendan Eich, un programador que trabajaba en Netscape, pensó que podría solucionar este problema adaptando otras tecnologías existentes (como ScriptEase) al navegador Netscape Navigator 2.0, que iba a lanzarse en 1995. Inicialmente, Eich denominó a su lenguaje LiveScript.  
🧑🏻‍💻  
Posteriormente, Netscape firmó una alianza con Sun Microsystems para el desarrollo del nuevo lenguaje de programación. Además, justo antes del lanzamiento Netscape decidió cambiar el nombre por el de JavaScript. La razón del cambio de nombre fue exclusivamente por marketing, ya que Java era la palabra de moda en el mundo informático y de Internet de la época.  
🖥️  
Más info [aquí](https://uniwebsidad.com/libros/javascript/capitulo-1/breve-historia)
