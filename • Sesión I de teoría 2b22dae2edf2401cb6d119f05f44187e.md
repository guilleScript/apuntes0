# **¿Qué son las ciencias de la computación?**
> En esta lección introductoria se verá qué son las Ciencias de la Computación, conceptos y algunas técnicas distintivas del campo y algunos antecedentes históricos relevantes.

## **Computación**

Presentación PDF: **[Ciencias de la computación](https://drive.google.com/file/d/1Ac2aq1M6E0d815OurvM7pE-KsAULVefV/view?usp=sharing)**

Video: [Computación](https://youtu.be/2j3kxsQrZU4)

> Lo que queremos es resolver problemas y automatizar esas soluciones. Por ello además de la computadora, el cuaderno es una herramienta esencial para nuestro trabajo. (diseñar)


> 💡 **Definición** Una **computadora** es una máquina electrónica capaz de almacenar información y tratarla automáticamente mediante operaciones matemáticas y lógicas controladas por programas informáticos.


- El objetivo principal de las computadoras es que **resuelvan problemas, de forma automatiza.**

> 💡 **Definición** Un **programa** es una secuencia de instrucciones que le indica a la computadora cómo resolver un problema.

> 💡 **Definición (Computación):** La disciplina de la computación es el estudio **sistemático** *(se estudia el problema de manera formal, sistemática. Para encontrar soluciones eficientes)* de procesos algorítmicos que **describen** *(para llegar a soluciones primero necesito información del problema, describirlo)* y **transforman información** *(que es la solución del problema)*: *(para hacer lo anterior se necesita:)* su **teoría**, **análisis**, **diseño** (*este es un campo muy creativo)*, **eficiencia** *(queremos encontrar soluciones y además que sean las mejores posibles, incluso evaluamos la calidad de nuestras soluciones)*, **implementación** *(nos interesa encontrar la solución valiéndonos de las matemáticas muchas veces, pero además nos interesa describirlas con algoritmos de manera que las computadoras puedan resolverlas, queremos aterrizar esas soluciones a problemas concretos)* y **aplicación**.

</aside>

*La pregunta fundamental subyacente en toda la computación es ¿qué puede ser (eficientemente) automatizado?” (que familias de problemas pueden ser modelados de forma algorítmica para ser aplicados a escenarios concretos). -Peter Denning, 2005*

**La computación tiene dos raíces fundamentales:**

1. La búsqueda de una sistematización del pensamiento. Es decir, la búsqueda de algoritmos para resolver problemas, algunas veces generales y otras concretos.
2. La búsqueda para desarrollar implementos o medios que permitan realizar cálculos de manera precisa y eficiente.

## **Algoritmos y funciones**

Video: [Algoritmos y funciones](https://youtu.be/MzVSHXMY3dg)

<aside>
💡 Definición (Algoritmo):Un algoritmo es una secuencia de pasos que transforma un valor o conjunto de valores, conocidos como entradas, en un valor o conjunto de valores, conocidos como salidas, de tal modo que éstas satisfagan un conjunto de relaciones *(características o condiciones que debe cumplir el algoritmo al buscar la solución para considerarse valida)* previamente especificadas. *(es una definición formal del análisis y diseño de las soluciones que vimos previamente).*

</aside>

![Untitled](%E2%80%A2%20Sesio%CC%81n%20I%20de%20teori%CC%81a%202b22dae2edf2401cb6d119f05f44187e/Untitled.png)

Las fórmulas matemáticas son, por ejemplo, algoritmos; son generales, lo que varía son los valores (entradas y salidas). (como una receta determinista).

<aside>
💡 **Definición (Función)** *(retomado de las matemáticas).* Una función recibe un conjunto de argumentos y produce un único resultado que depende de esos argumentos.

</aside>

![Untitled](%E2%80%A2%20Sesio%CC%81n%20I%20de%20teori%CC%81a%202b22dae2edf2401cb6d119f05f44187e/Untitled%201.png)

En principio son lo mismo, es como un algoritmos en su sentido matemático, la diferencia es que cuando hablamos de una función se habla de un ente más general y abstracto, incluso implícito lo que está dentro de la función y como es que devuelve el resultado, mientras que en un algoritmo si se tiene explícitamente una secuencia de pasos que nos dice como transformar las entradas en las salidas, lo que está en la cajita. Entonces un algoritmo es la **especificación** de una función.

La función nos ayudará para el estudio teórico de el problema general (si existe, si podemos guiarnos en algo para encontrar el algoritmo, etc.), incluso antes de tratar de encontrar el algoritmo concreto.

En general cuando hablemos de algoritmo nos referimos a que describe una secuencia de pasos lógicos, mientras que una función puede ser considerada como uno de esos pasos y se enfoca en la transformación de las entradas en salidas, sin necesidad de detallar su implementación interna.

## **Complejidad**

Video: [Complejidad](https://youtu.be/bNeIUwawiGg)

Habíamos dicho que no solo nos interesa encontrar una solución sino encontrar la más eficiente posible, o al menos razonablemente eficiente, dependiendo del problema. Para ello nuestra forma de medir que tan eficientes son esas soluciones es lo que trata el concepto de **complejidad**.

Por **complejidad** nos referimos en forma genérica a las diversas características que señalan el desempeño de un algoritmo:

1. **Tiempo:** ¿cuánto tarda en ejecutarse un algoritmo?, ya sea con seg, horas, meses, años, etc. Se pregunta sobre todo **cuantas instrucciones se debe ejecutar para resolver el problema**, así podemos medir nuestro tiempo independientemente de la maquinaria en la que se esté trabajando.

2. **Espacio:** ¿cuánta memoria utiliza para su ejecución?, para los datos que están siendo manipulados para encontrar la solución del problema, datos residuales, etc. Entre menos espacio usado para datos mejor.

3. **Tamaño:** número de instrucciones. El tamaño del código perse, cuantas líneas de código ocupa mi algoritmo, pero es diferente al tiempo, porque puede que el tamaño sea pequeño, porque escribí pocas líneas, pero si mi última instrucción dice repita las anteriores 1000 veces, entonces en tiempo es poco eficiente. O por ejemplo, un algoritmo que tenga muchos if, muchas opciones diferentes dependiendo de los datos de entrada, pero que al elegir uno se ejecuten pocas líneas de código, en este caso en **tamaño** no es tan pequeño o eficiente pero en **tiempo** puede que sí. Igual, entre menos mejor también para leer.

4. **Dificultad:** ¿qué tan complicado es de leer, entender, modificar y extender?. Indentación, comentarios, se entiende (por mí y por otros programadores), se puede extender, etc.

## **Modelos teóricos**

Video: [Modelos teóricos](https://youtu.be/63TEKJX9kiY)

Nos sirven para estudiar el problema a resolver así como la maquinaria sobre la que se aplicará la solución.

### **1. Análisis de Algoritmos**

Si, por ejemplo, tenemos el problema a resolver y hemos encontrado la solución (hemos diseñado el algoritmo), a través del análisis de algoritmos podemos estudiar esa solución antes siquiera de haberlo escrito en un lenguaje en específico y en un hardware específico.

> Se desea predecir el comportamiento del algoritmo sin implementarlo en una máquina específica. Udi Manber
> 

Para ello se **modela** a las computadoras como máquinas de operaciones elementales. **Creamos un modelo teórico** de una computadora con operación matemáticas básicas que son la base de ella, esto porque las computadoras reales incluyen operaciones compuestas más complejas (al variar el procesador, gpu, ram, etc.) que generan variaciones en la ejecución de nuestro algoritmo,  pero lo que nosotros queremos es abstraernos de ello, para poder analizar el problema y el algoritmo independientemente de esas variaciones de hardware.

- Un modelo de cómputo es un conjunto de suposiciones/reglas sobre:

1. las operaciones elementales que puede realizar una computadora,
2. el tiempo que le tomará ejecutarlas,
3. la forma en que almacenará los datos en memoria.

<aside>
💡 Este modelo es suficientemente sencillo para analizar mis algoritmos sin preocuparme por la implementación en determinado hardware.

</aside>

> Se utilizan estos modelos para evaluar la complejidad de los algoritmos, independientemente de la maquinaria física que los ejecute.
> 

Lo importante es ser independiente a la tecnología utilizada. De esta manera puedo estudiar problemas complejos y hacer más eficiente los algoritmos independiente a la tecnología, lo que se busca son las propiedad matemáticas inherentes del problema.

Esto nos ayudó a ver, por ejemplo, que sin importar que tan avanzada y potente hagamos una máquina en el futuro, hay problemas que son imposibles de resolver, por lo menos no con las metodologías actuales. También nos ayuda a ver si se puede mejorar la complejidad (tamaño, tiempo, etc.) del algoritmo antes de implementarlo, independiente del hardware.

Una vez hemos pasado esta etapa que nos dice si nuestra solución es la más eficaz, o lo suficientemente eficaz, ya podemos implementarlo en un lenguaje.

## **Teoría de la Computación**

**¿Qué estudia la teoría de computación?**

> En teoría de la computación se abstrae el concepto de “computadora”, pensándola como una función (como el ente matemático que vimos) y se estudia su capacidad para resolver problemas.
> 

Al respecto Viso G. 2008 plantea las preguntas siguientes:

- ¿Qué quiere decir que una función sea computable? ¿Qué tipos de funciones son computables? (no todo es computable o no al menos en un tiempo razonable)
- ¿Qué tanto podemos decir de las que no lo son? (por qué no se pueden unas y otros no)
- ¿Cómo están relacionadas las construcciones en lenguajes de programación con el poder de cómputo? (como afecta la sintaxis de una lenguaje a su capacidad de resolver(describir) mejor unos problemas que otros).
- ¿Qué hace que algunos problemas sean computacionalmente difíciles de resolver (requieren demasiados cómputos(cálculos))? (a veces no hay algoritmos eficientes u otros que no existen, que no hay solución algorítmica)
- ¿Podemos caracterizar a las funciones que no pueden ser calculadas eficientemente? (encontrar por qué no pueden ser computables)

Por ejemplo, en teoría de la computabilidad y en teoría de la complejidad computacional, un **problema indecidible** es un problema de decisión para el cual es imposible construir un algoritmo que siempre conduzca a una respuesta de *sí* o *no* correcta. El problema de la parada es un ejemplo: no existe algoritmo que determine de manera correcta si un programa arbitrario se detendrá, una vez sea ejecutado...

Al ejecutar un conjunto de programas, este puede terminar después de un número finito de pasos o puede no terminar nunca. En la práctica, este último caso se manifiesta como programas que se quedan «*trabados*» o que entran a un bucle infinito. Por esta razón sería de gran utilidad resolver la siguiente pregunta en la práctica:

> Existe un programa P, tal que, dado un programa cualquiera q y unos datos de entrada x, muestre como salida 1 si q con entrada x termina en un número finito de pasos o muestre como salida 0 si q con x entra a un bucle infinito.
> 

Conocer si existe el programa *P* es, en términos resumidos, el problema de la parada.

Sin embargo, hay que hacer notar que la sabiduría popular acerca de este problema hace pensar que nunca es posible demostrar que un programa termina. Esto es falso.

Lo que se afirma es que **no existe una manera automática computable de saber si todos los programas posibles terminan. No se niega que exista la prueba para programas concretos**. De hecho, la construcción de pruebas para programas concretos es un paso obligatorio para demostrar su correctitud. (osea que en el caso general no se puede crear ese P, pero en casos específicos sí).

El procedimiento para construir estas pruebas no es automático; sin embargo, existen heurísticas *(estrategias, reglas)* que facilitan encontrar las pruebas de los programas. El área de conocimiento que estudia la construcción sistemática de pruebas se denomina *Análisis de Terminación.* La evaluación o ejecución del programa con las entradas sin embargo no constituye una prueba de que siempre termine, sino de que, en las circunstancias de la ejecución, terminó.

## **Disciplinas semejantes**

Video: [Disciplinas semejantes](https://youtu.be/9odcE7qMVhg)

1. **Programación** 

<aside>
💡 “La programación consiste en elaborar un algoritmo, escrito en un lenguaje susceptible de ser ejecutado por una computadora y para resolver una clase de problemas.” Viso y Peláez V. 2012

</aside>

*Es la parte de escribir y diseñar. Las CC abarcan mucho más como analizar, caracterizar, optimizar, etc., más teoría. Pero también lo incluye.*

1. **Ingeniería de la computación**

Dependiendo de la Universidad donde se imparta la carrera, incluso puede llegar a ser intercambiable con Ciencias de la computación

Tiende a poner más énfasis en el diseño y funcionamiento del equipo mecánico (hardware), programación de dispositivos electrónicos y, por consiguiente, en lenguajes de programación más cercanos a él, como los ensambladores. *CC se enfoca más en el análisis matemático de los problemas y en la calidad de las soluciones, nos alejamos más del hardware.*

1. **Cibernética**

Surge en 1942 es impulsada inicialmente por Norbert Wiener y Arturo Rosenblueth Stearns.

Inspirada en los sistemas de autorregulación biológicos, plantea el diseño de sistemas mecánicos que interactúen con su ambiente guiados por una función de equilibrio. Cuando el equilibrio se rompe, responden con acciones que tienden a recuperar el equilibrio.

Encuentra su aplicación natural en campos como la robótica **(como un cuarto que autorregula su temperatura para encontrar el equilibrio)** y la percepción remota.

1. **Informática**

Cubre los aspectos de la computación relacionados directamente con la administración de la información:

- Sistemas de información,
- bases de datos.

Incluye aspectos de administración no exclusivos de la computación.

Enfocados al ambiente empresarial y administrativo, por ello muy útiles en las empresas, pero no se preocupan por análisis de algoritmos ni nada de eso.

1. **Tecnologías de la información y Ciencia de datos (big data)**

Se preocupa de las formas de:

- Manejar,
- transmitir,
- procesar la información.

En épocas recientes, se caracteriza por la aplicación de técnicas de inteligencia artificial y aprendizaje de máquina para extraer información a partir de grandes cantidades de datos.

![Untitled](%E2%80%A2%20Sesio%CC%81n%20I%20de%20teori%CC%81a%202b22dae2edf2401cb6d119f05f44187e/Untitled%202.png)

# Lenguajes de programación

Presentación PDF: **[Lenguajes de programación y sus paradigmas](https://drive.google.com/file/d/1-MzHshscEU2JgZbD8xmAcWtpEYXB5KOV/view?usp=sharing)**

Video: [Paradigmas](https://youtu.be/fLZUBwbVLXY)

## **Paradigmas**

¿Cuántos lenguajes de programación existen?:  Según el **Blog del Centro de e-Learning**, existen cerca de **700 lenguajes de programación** distintos, cada uno con un fin y una orientación diferente. 

¿En qué lenguaje programa un computólogo? — ¡En el que le pidan!

— ¿Cómo le hace?

— **Estudiando paradigmas**

De esta manera podemos entender el funcionamiento profundo del lenguaje lo podemos intuir por el paradigma al que pertenece, por lo que podemos ver que las diferencias pasan a ser principalmente de sintaxis y particularidades, lo que facilita mucho las cosas.

<aside>
💡 Cada **paradigma de programación** describe:

</aside>

1. Una **filosofía y metodología** para crear programas para la computadora.
2. Esta filosofía define la forma de conceptualizar a la información que será procesada (cómo afronta el problema, la filosofía), así como 
3. el formalismo y reglas para operar con esa información (sintaxis del lenguaje, semántica, etc.), permitiendo calcular resultados que satisfagas las condiciones establecidas.

> *La semántica significa el estudio del significado de los signos lingüísticos matemáticos. Por ejemplo, analicemos la palabra TUNA. La sintaxis (como reglas gramaticales generales)es la secuencia de las cuatro letras en orden, pero su semántica (su fondo, su significado y si tiene sentido independientemente de que sea sintácticamente correcto)puede variar. Por ejemplo, en español es el fruto del nopal y en inglés es un pescado.*
> 

Recientemente se han propuesto varios paradigmas, pero mencionaremos aquí los referentes fundamentales.

<aside>
💡 El objetivo durante la carrera es aprender a programar bien en un lenguaje de cada paradigma.

</aside>

## **Declarativo, imperativo y orientación a objetos**

Video: [Declarativo, imperativo y orientación a objetos](https://youtu.be/4iXWT2XO5n0)

### **Paradigma Imperativo vs Declarativo:**

1. **Lenguajes imperativos:** *(HISTÓRICAMENTE EL PRIMERO)*
    1. Especifican (a la computadora) el qué y el cómo se debe hacer.
    2. Están inspirados en la estructura física de la computadora. (puede depender del hardware específico de cada computadora).
    3. La memoria o estado se visualiza como un conjunto de asociaciones entre posiciones de memoria y los valores almacenados en esas posiciones. (definición y asignación de variables, por ejemplo).
    4. Un programa consiste en una serie de comandos que indican cómo y cuándo almacenar y procesar valores en las posiciones de memoria. (manipular las variables o posiciones de memoria).
    5. *Por tanto en este tipo de lenguajes damos instrucciones a la computadora directamente, es como si usáramos oraciones imperativas de órdenes. Por ejemplo, como visualizamos las posiciones de memoria como una cinta con cajas en las que entran valores, estos lenguajes afrontan los problemas con instrucciones tipo; mueve el valor de la posición a la posición b, borra tal valor de esa posición, etc.*
    6. Ejemplos: Fortran, Pascal, C, Java, Python.

1. **Lenguajes declarativos:**
    1. Se basan en el principio de que la programación **debe** enfocarse en indicar lo que se debe hacer, mientras que el intérprete del lenguaje se encarga de resolver el **cómo** llegar al resultado deseado.
    2. Este ideal, en su forma pura, produce programas menos eficientes.
    3. *Nos libera de una parte del trabajo. Como vimos antes, al especificar el algoritmo establecemos unas series de relaciones (condiciones) o restricciones que queremos que se cumplan para dar por resuelto el problema, entonces en estos lenguajes (su filosofía) lo importante es especificar correctamente que es lo que queremos (a lo que se debe llegar), une vez hecho eso podremos usar un programa previo (intérprete) que sigue reglas lógico-matemáticas que dadas mis especificaciones pueda resolver él como llegar a la solución.*
    4. Están inspirados en las notaciones matemática y lógica.
    5. En sus versiones puras, no hay variables modificables ni comandos para modificar su estado. (a diferencia del imperativa que se basa en eso).
    6. Un programa consiste en un conjunto de declaraciones de funciones o relaciones que definen valores nuevos.
- Los l**enguajes declarativos s**e dividen en dos clases:
    1. **Funcionales**: consiste en la evaluación de funciones siguiendo reglas como la composición y aplicación (o evaluación) en forma semejante a las funciones de cálculo. *(nosotros definimos funciones que el programa usa para llegar a la solución, como f(x), el clásico ejemplo del factorial…)*
        - Ejemplos: Scheme, ML, Haskell.
    2. **Lógicos**: los cómputos están basados en deducciones según las reglas de la lógica de primer orden. *(predicados con variables y constantes y lo que hace es tratar de llegar a los valores de las variables indicados para que las afirmaciones que hayamos puesto sean correctas)*
        - Ejemplo: Prolog.

### **Lenguajes orientados a objetos:**

> Aplica para lenguajes imperativas y declarativos, más común en el primero. Necesario debido a que se aumentó mucho la complejidad de los sistemas (crisis del software), se necesitaba escalar el código.
> 

<aside>
💡 Se trata de un paradigma orientado hacia lograr **la correcta organización de sistemas vastos y complejos** mediante el uso de ***clases y objetos. -**Divide y vencerás, dividir en partes autónomas que se comunican en los sistemas complejos.*

</aside>

Abstraen el concepto de tipo de dato a manipular según:

1. El conjunto de datos admisibles dentro de cada tipo. (atributos de los datos de la clase)
2. Las operaciones que se pueden realizar con ellos. (métodos de la clase)

<aside>
💡 **Encapsulamiento**, delimitando estrictamente las fronteras entre operaciones permitidas entre tipos de datos distintos. *La autonomía de cada unidad, que la hace independiente a las demás por lo que no debe interferir en las operaciones y datos de la otra. Ya después interactúan las diferentes clases entre sí.*

</aside>

<aside>
💡 Reutilizamiento del código mediante el mecanismo de **herencia** (se especifican diferencias pero heredan código de otra clase)

</aside>

- Ejemplos: **Java, Python, Ruby.**

## **Los 4 paradigmas y algunos lenguajes**

Video: [Los 4 paradigmas y algunos lenguajes](https://youtu.be/-Zb7v6nuBZE)

![Untitled](%E2%80%A2%20Sesio%CC%81n%20I%20de%20teori%CC%81a%202b22dae2edf2401cb6d119f05f44187e/Untitled%203.png)

- Los lenguajes muchas veces tienen a invadir otros paradigmas, casi no hay puros, imperativos o declarativos, etc.
- Empezar con java es bueno porque nos da disciplina y buenas prácticas para poder programar sistemas complejos y escalables gracias a su formalidad, lo que después podremos trasladar a otros lenguajes que no requieren esa formalidad en un inicio.
- **Haskell** es funcional también y cada vez más importante.
- Las materias de matemáticas nos ayudan a entender estos lenguajes, el imperativo se parece al álgebra. El Funcional a cálculo y álgebra y el lógico a la lógica (como álgebra superior), etc.
