*MÓDULO SOBRE LÓGICA, LÓGICA DE PROGRAMACIÓN Y PROGRAMACIÓN CONJAVASCRIPT*

# Preguntas teóricas

1. ¿Qué es la lógica en el contexto de la programación? Y explicar por qué es importante
en el desarrollo web Frontend. 
 
 R//: la lógica de programación es la facultad de dar instrucciones y construir soluciones coherentes para lograr una página web bien constituida o alcanzar un objetivo deseado.

 2. Definir el concepto de “algoritmo” y proporcionar un ejemplo sencillo de un algoritmo
relacionado con la lógica de programación. 
 
 R//: Es una sencuencia lógica de pasos para llegar un fin establecido.
 R//: Cambiar una lámpara

 3. ¿Qué son estructuras de control en la programación?, ¿Cuáles son los tipos de estructuras de control y las estructuras más comunes de cada tipo?, Describir al menos dos tipos de estructura de control, explicar por qué son importantes y proporcionar ejemplos de cada uno de cómo se utilizan en el desarrollo web Frontend. 
 
 R//: Las estructuras de control son elementos que nos permiten modificar el flujo de ejecución de un programa y los tipos de estructuras de control son secuenciales, condicionales y cíclicas. 
    *Secuenciales:* estas estructuras implican un orden secuencial de instrucciones, es decir, se suceden unas con otras y la entrada de una tarea, es la salida de otra.
    *Condicionales* estas estructuras de control permiten relizar acciones dependiendo de la condición si es falsa o verdadera. 
    *Ejemplo*: 
    - If-else: sirve para tomar decisiones basadas en una condición y por ende, se ejecuta un código si se cumple la condición. Es imporante en el desarrollo frontend, ya que permite interactividad, acciones,control de flujo de la apliación y una mejor experiencia del usuario, como por ejemplo datos de formulario, validar entradas de usuario, entre otras.
    - Switch-case: es similar a la anterior pero su caracerística principal es que se utiliza cuando son varios casos a evaluar. Es muy necesaria para manejar diversos casos y tomar decisiones basadas en múltiples valores. De tal modo, es eficaz para procesar entrar de usuario, adaptar interfaz a diferentes estados o regular flujos muy complejos en la web.
    *Iterativas o de repetición* Son también conocidas como bucles y permiten ejecturar bloques de código a la par de que se cumple una condición dada. Facilita la vida de tareas repetitivas. 
    *Ejemplo*: 
    - For: este se utiliza para iterar un número específico de veces. Por ende, el ciclo for es esencial, puesto que permite trabajar con datos, manipular el DOM, generar contenido dinámico y crear interacciones y efectos visuales  eficiente y organizadamente, lo que contribuye a la construcción de interfaces web dinámicas y atractivas.
    - While: este ciclo repite un bloque de código mientras una condición sea verdadera. Asimismo, el bucle while es relevante en el desarrollo frontend porque permite controlar el flujo de ejecución de manera dinámica, esperar eventos o condiciones específicas, y manejar casos donde se necesite una ejecución continua hasta que se cumplan ciertas condiciones.
    - Do-while: este es similar al while, pero el código se ejecuta al menos una vez y luego verifica la condición para determinar si se debe seguir repitiendo ese bloque de código. El bucle en cuestión, en el desarrollo frontend, es útil porque asegura la ejecución de un bloque de código al menos una vez y luego verifica una condición. Esto es provechoso en momentos donde se requiere realizar una acción inicial o esperar eventos o datos dinámicos, antes de verificar y continuar con la ejecución del código basado en condiciones específicas.

4. Describir cómo se declaraban variables y constantes en JavaScript antes de la introducción de ECMAScript 6 (ES6). Explicar cómo ES6 mejoró la declaración de variables y constantes, y mencionar los problemas que esta mejora resuelve en el desarrollo web Frontend. 

R//: Antes del ECMAScript6, las variables se declaraban con *var*. Esta declaración tenía un ámbito de función y no de bloque. Por otro lado, las constantes no existían, pero había una convención que comúnmente se utilizaba al declarar constantes y era utilizando los nombres en mayúsculas y subrayados. En ese sentido, ECMAScript 6 hizo mejoras considerables e introdujo *let* y *const*, la primera cobra sentido cuando vamos a declarar variables con un alcane de bloque y la segunda, se utiliza para declarar variables cuyo valor es inmutable. El uso de let y const ha proporcionado la resolución de varios aspectos en la programación, como por ejemplo, los errores relacionados con el ámbito de función, la reasignación accidental de valores, el hoisting, problemas con bucles, entre otros.

5. ¿Cómo se declaran las funciones en JavaScript y cuál es la diferencia entre una declaración de función, una expresión de función y una función de flecha (arrow function)? Proporcionar ejemplos de cada una. 
 R//: Las funciones en JavaScript se declaran utilizando la palabra clave *function* seguida de una espacio, luego el nombre de la función, al estar ya definido su nombre introducimos entre paréntesis las variables y parametros que deseamos para dicha función, posterior a esto tendremos lo que sería el cuerpo de la función introducido por llaves {}
 *Ejemplo*: 
 function resta(a, b) {
  return a - b;
}

La diferencia que existe entre una declaración de función, una expresión de función y una función de flecha (arrow function) es que la declaración de función se define con la palabra clave function, tiene su propio ámbito y puede ser llamada antes de su definición (hoisting). Luego está una expresión de función que asigna a una variable con la palabra function, pueden ser anónimas. Posteriomente está la arrow function que fueron introducidas en ECMAScript 6 (ES6) y tiene unos comportamientos diferentes a las funciones tradicionales, como por ejemplo, no tiene argumentos propios, no pueden ser usadas como constructores y por otro laddo, no tienen su propio this, pero utilizan el this del contexto que lo rodea en el momento en que se definie la función.

*Ejemplo*
- Declaración de función:   
  function suma(a, b) {       
  return a + b;
}

console.log(suma(10, 5)); 

- Expresión de función:
const multiplicacion = function(a, b) {
  return a * b;
};

console.log(resta(40, 3));

- Arrow function
 const saludar = () => "¡Hola Mundo!";

  console.log(saludar());

6. ¿Por qué es necesario el uso de funciones en el desarrollo web Frontend? Enumerar al menos tres razones fundamentales y proporcionar ejemplos de situaciones en las que las funciones son esenciales. Además, mencionar la ventaja de las funciones flecha en el contexto de estas razones. 

R//: La  funciones juegan un papel fundamental en el desarrollo web Frontend, ya que nos permite reutilizar código, a tener un código más limpio, estructurado y ordenado y también a tener una buena modularización. Las funciones tienen una serie de ventajas en cuanto a sintaxis más concisa y reducir la líneas de código.

7. ¿Cuál es la diferencia entre parámetro y argumento?

R//: La diferencia es que el parámetro es el valor utilizado en la definición de una función y el argumento es el valor real que se le pasa a la función cuando es invocada. 

8. Definir el concepto de Callback y proporcionar un ejemplo práctico. 

R//: Un callback es una función que se pasa como argumento a otra función, es decir, es una función que se llama de vuelta en líneas posteriores en el código. 

*Ejemplo* :
Fuente: https://developer.mozilla.org/es/docs/Glossary/Callback_function

function saludar(nombre) {
  alert("Hola " + nombre);
}

function procesarEntradaUsuario(callback) {
  var nombre = prompt("Por favor ingresa tu nombre.");
  callback(nombre);
}

procesarEntradaUsuario(saludar);

9. ¿Qué es el hoisting en JavaScript y cómo afecta a las variables y funciones? Proporcionar ejemplos de hoisting en declaraciones de variables y funciones. 

R//: El término hoisting en JavaScript se utiliza para describir que las declaraciones de variables y funciones son movidas al inicio de su ámbito de alcande antes de que se ejecute el código. El hoisting sólo aplica para variables declaradas con var, con let y const no funciona.
*Ejemplo*: 

- console.log(miVariable); 
var miVariable = 10;

- console.log(miConstante);
const miConstante = 5;

- saludar(); 

function saludar() {
  console.log('¿Cómo está?');
}

10. Definir brevemente el concepto de objeto en JavaScript y cuál es la visión general este concepto. Indicar, también cómo se declaran estas estructuras de datos. 

R//: Un objeto, a modo general, es una estructura de datos que permite almacenar datos y funciones como propiedades y métodos. Consisten en pares clave-valor que posibilitan almacenar información.

const automovil = {
  marca: 'Toyota',
  modelo: 'Corolla',
  año: 2019,
};

11. ¿Qué son propiedades?, y ¿Cuál es la diferencia entre una propiedad y un método en un objeto?

R//: Las propiedades son los valores asociados a un objeto, representando caraterístias y datos. Por otro lado, un método está relacionado con las funciones y estas a su vez están ligadas con el comportamiento o las acciones que el objeto puede llevar a cabo.

12.  Explicar las dos formas de acceder a una propiedad de objetos e indicar las situaciones
en que conviene usar una manera sobre la otra.

R//: Existen dos formas de acceder a una propiedad, la primera es por medio de notación de puntos *objeto.propiedad* y la segunda, es por medio de la notación de corchetes *objeto['propiedad']*

13. ¿Existe alguna forma de recorrer las propiedades de un objeto? En caso negativo, explicar por qué no es posible y en caso positivo proporcionar un ejemplo. Mencionar una situación en la cual sea muy útil recorrer las propiedades de un objeto. 

R//: Si, existen unas formas más comúnes de recorrer las propiedades de un objeto, una por medio de un bucle for...in y la otra es por medio de un método como Object.keys(). 
Una de las situaciones útiles para recorrer las propiedades de un objeto es cuando se está trabajando con datos dinámios o con objetos JSON. 

*Ejemplo*: 
- For...in
const persona = {
  nombre: 'Alejandro',
  edad: 29,
  profesion: 'Docente'
};

for (let propiedad in persona) {
  console.log(propiedad + ': ' + persona[propiedad]);
}

- Object.keys() 
const persona = {
  nombre: 'Alejandro',
  edad: 29,
  profesion: 'Docente'
};

const propiedades = Object.keys(persona);
propiedades.forEach(propiedad => {
  console.log(propiedad + ': ' + persona[propiedad]);
});

14. ¿Por qué son útiles los objetos en la programación web y qué tipos de datos pueden almacenar? 

R//: Los objetos son útiles en la programación web, puesto que tiene características fundamentales como organizar y estructuras datos de manera adecuada, manipulación con el DOM y comunicación con otros servicios externos.

Algunos tipos de datos que se pueden almacenar: 
- Cadenas de texto
- Arrays
- Funciones
- Booleanos
- Números

15. ¿Qué es un array en JavaScript y por qué son esenciales?

R//: Un array en JavaSript es una estructura de datos que sirve para almacenar varios elementos, además, es una colección ordenada específicamente y permitiendo una manipulación eficiente de elementos. 
Los array son esenciales para almacenar datos, iterar y tener interacción con APIS y otros servicios web. 

16. ¿Cómo acceder a un elemento dentro de un array? Explicar con un ejemplo.

R//: En los arrays cada elemento tiene una posición y está representada por un índice numérico. Debemos tener en cuenta que se parte desde el 0 ()cero al momento de la impresión del dato. Para acceder aquí está un ejemplo: 

const estudiantes = ['Camilo', 'Pedro', 'María', 'Carlos'];

console.log(nombres[2]); // Imprimirá 'María'

17.  Mencionar al menos tres funciones de arrays y describir su utilidad en la programación  web.

R//: También son conocidas como métodos de array: 
- map(): devuelve un array actualizado bajo una condición dada.
- filter(): se utiliza para crear un nuevo array con los elementos que cumplan con la condición 
-find(): se utiliza para busar y devolver el primer elemento que coincida con la condición especificada. 

18.  Proporcionar un ejemplo de cómo se utiliza una función de array para transformar y  filtrar datos en un array.
 
 R//: 
 const productos = [
  { nombre: 'Camisa', precio: 25 },
  { nombre: 'Jean', precio: 70 },
  { nombre: 'Zapatos', precio: 90 },
  { nombre: 'Morral', precio: 15 },
  { nombre: 'Chaqueta', precio: 150 }
];

const productosCaros = productos
  .filter(function(producto) {
    return producto.precio >= 50; // Filtrar los productos con precio mayor a $50
  })
  .map(function(producto) {
    return { nombre: producto.nombre, precio: producto.precio }; // Crear objeto solo con nombre y precio
  });

console.log(productosCaros);


*MÓDULO SOBRE HTML, CSS Y RESPONSIVE DESIGN*

# Preguntas teóricas

1. ¿Qué significa HTML y cuál es su función en el desarrollo web?

R//: HTML significa "HyperText Markup Language" (Lenguaje de Marcado de Hipertexto) y tiene varias funciones en el desarrollo web como por ejemplo proporcionar una estrtuctura básica para organizar una página web, permite crear enlaces con otras páginas web, permite una distribuión semántica de las etiquetas, tiene una amplia compatibilidad y accesibilidad con navegadores, entre muchas otras.

2. ¿Cuál es la estructura básica de un documento HTML? Describir las etiquetas esenciales.

R//: 
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Proyecto HTML</title>
</head>
<body>
  
</body>
</html>

<!DOCTYPE html> : la versión de HTML que se está utilizando.
<html lang="es"> : Es la etiqueta raíz que envuelve todo el contenido de la página web y *lang="es"* se refiere al lenguaje.
<head> : Dicha sección alberga metadatos y enlaces a recursos externos, como el título, enlace a CSS, scripts, entre otros. 
<meta charset="UTF-8"> : juego de caracteres utilizado en el documento.
<body> : El cuerpo de la página web. Contiene una amplia gama de contenido de la página web, como por ejemplo texto, imágenes, enlaces, formularios, entre otros.

3. ¿Qué es CSS y cuál es su propósito en el desarrollo web?

R//: 
CSS significa "Cascading Style Sheets" (Hojas de Estilo en Cascada) y es un lenguaje utilizado para describir la presentación y el aspecto visual de un documento HTML o XML.
Su propósito es mejorar la apariencia visual, los estilos de las páginas web y tener una mayor presentación en diferentes plataformas. 

4. ¿Qué son selectores CSS, cuáles son los principales tipos de selectores y porqué es importante entender la especificidad en el contexto de las hojas de estilo en cascada (CSS)? Describir al menos tres tipos de selectores CSS y cómo la especificidad afecta a la aplicación de estilos en un proyecto de desarrollo web Frontend. Proporcionar ejemplos de situaciones en las que se utiliza la especificidad de selectores para resolver conflictos de estilos. 

R//: 
Los selectores CSS son patrones que se utilizan para aplicar estilos a elementos HTML propios de una página web. Estos permiten dirigirse a los elementos y definir cómo deben de lucir y comportarsen.
Los principales selectores son de tipo (h1, span, p, div), de clase (.class) y selectores de ID (#identificador)

Por otro lado, la especificidad determina la prioridad de unos estilos sobre un mismo elemento. Se calcula según la combinación de selectores. Por ejemplo, si se aplica un estilo con ID y otro con una clase al mismo elemento, en ese caso el ID tiene más especificidad y se aplicarán los correspondientes estilos por encima de la clase.

5. Explicar las diferencias entre los estilos en línea (inline), estilos internos (embedded) y estilos externos (external) en CSS. Indicar cuál de los tres estilos es el recomendado usar y por qué. 

R//: 
*Estilos en línea (Inline)*:
Se aplican directamente a elementos individuales dentro de HTML usando el atributo style.

<p style="color: red; font-size: 10px;">Estilos en línea.</p>

*Estilos internos (embedded)*
Los estilos internos son reglas de estilo CSS que se definen dentro del documento HTML con la etiqueta <style> y se ubican dentro de la etiqueta <head>.

<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Proyecto HTML</title>
  <style>
    p {
      color: blue;
      font-size: 15px;
      justify-content: center;    
      }

    h1 {
      color: green;
      font-size: 24px;
    }
  </style>
</head>
<body>
  <h1>Estilos Internos</h1>
  <p>Lorem ipsu</p>
</body>
</html>

*Estilos externos*:

Los estilos externos son los que se definen en otro archivo por medio de una extensión .css, se vinculan en el documento utilizando la etiqueta <link> dentro del <head>

<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Proyecto HTML</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <h1>Estilos Internos</h1>
  <p>Lorem ipsu</p>
</body>
</html>

6. ¿Qué es flexbox y cómo se utiliza para el diseño de páginas web?

R//: 
Flexbox es un módulo de diseño de CSS que permite la creación de diseños web más flexibles y adaptables sobre todo cuando de contenedor se trata. 

Se utiliza *display: flex* para activar diseño flexbox.

7. Explicar cómo se emplean las propiedades flexbox y explicar la función de las principales propiedades en la creación de diseños flexibles.

R//: 
Las propiedades permiten el control, la alineación	y la distribución de los elementos en flexbos. Alguna de las propiedades son: 

- display: flex: Esta propiedad es para activar el diseño flexbox.
- flex-direction: se utiliza para definir la dirección de los elementos, puede ser row (de izquierda a derecha), column (de arriba a abajo).
- justify-content: permite alinear los elementos a lo largo del eje principal. Además distribuye el espacio entre los elementos con otros valores como (space-between), (flex-start), (flex-end), (center), (space-around).
- align-items: nos permite alinear los elementos a lo largo del eje transversal del contenedor. Se puede utilizar con los valores (stretch), (baseline), (center), (flex-end), (flex-start).

8. ¿Qué es CSS Grid Layout y en qué se diferencia de flexbox?

R//: 
CSS Grid Layout es un módulo diseño, posibilita crear diseños bidimensionales y se diferencia de flexbox, ya que este se centra en la creación de diseños unidimensionales.

9. Proporcionar un ejemplo de cómo crear una cuadrícula sencilla con CSS Grid.

R//: 
Un ejemplo de una cuadrícula con CSS Grid:

HTML:
<div class="container">
  <div class="item">1</div>
  <div class="item">2</div>
  <div class="item">3</div>
  <div class="item">4</div>
  <div class="item">5</div>
  <div class="item">6</div>
</div>

CSS:
.container {
  display: grid;
  grid-template-columns: 100px 100px 100px;
  grid-gap: 10px; /* Espacio entre las celdas */
}

.item {
  background-color: #f0f0f0;
  padding: 10px;
  text-align: center;
}

10. ¿Qué significa el diseño responsivo en el contexto del desarrollo web?

R//: 
El diseño responsivo en el contexto del desarrollo web, es la creación o la construcción de interfaces adaptables en diferentes pantallas y de igual manera que responda de forma óptima y fluida mejorando la experiencia del usuario y la accesibilidad del contenido.

11. Enumerar al menos tres técnicas o estrategias utilizadas para lograr el diseño responsivo en una página web. 

R//: 
Las técnicas o estrategias utilizadas para lograr el diseño responsivo en una página web son: 
- Media Queries
- Unidades de Medida Relativas (EM o REM)
- Multimedia Flexibles

*MÓDULO SOBRE DOM E INTERACCIÓN CON EL DOM*

# Preguntas teóricas

1. ¿Qué es el DOM (Modelo de Objeto de Documento) en el contexto de la programaciónweb? 

R//: El DOM representa una estructura jerárquica en forma de árbol, en él se puede interactuar y modificar la estructura, contenido y estilo de la página, lo que permite crear páginas web dinámicas e interactivas.

2. ¿Cuál es la diferencia entre el DOM y el HTML en una página web?

R//:
En resumidas cuentas, el HTML es la maquetación o el código que define la estructura inicial de una página web, mientras que el DOM es la representación dinámica generada por el navegador a partir de un documento HTML y puede ser manipulado por Javascript.

3. ¿Porqué es importante entender y manipular el DOM en el desarrollo web Frontend?

R//:

Entender y manipular el DOM en el desarrollo web frontend es fundamental porque posibilita crear páginas web dinámicas, actuliazaciones dinámicas, facilita la adapattabilidad a diferentes pantallas y dispositivos, propende a la construcción de interfaces sofisticadas, fluidas, complejas y permite una mejor experiencia del usuario.

4. ¿Qué son los eventos del DOM y cuál es su función en una página web?

R//:

Los eventos del DOM son acciones que se dan en una página web y estos se dan por la ejecución de los usuarios, el navegador u otros cambios. Su función en una página web es la interactividad, control de flujo y gestión de acciones. 

5. Proporcionar ejemplos de eventos prácticos y comunes, como “click”, “submit” y “load o DOMContentLoad”.

R//:

Ejemplos de eventos prácticos:

- 'click'
const button = document.getElementById('miBoton');
button.addEventListener('click', () => {
  console.log('¡Haciendo click en el botón!');
});

- 'submit'
const form = document.getElementById('miFormulario');
form.addEventListener('submit', (event) => {
  event.preventDefault();
  console.log('Formulario enviado');
});

- 'load'
window.addEventListener('load', () => {
  console.log('¡La página ha cargado completamente!');
});

- 'DOMContentLoad'
document.addEventListener('DOMContentLoaded', () => {
  console.log('¡El DOM ha cargado!');
});

6. ¿Por qué es importante manejar eventos en la interacción usuario-web y cómo se añaden controladores de eventos a los elementos del DOM?

R//:

Los eventos facilitan una experiencia interactiva entre el usurio y la web y por otro lado permiten que la página web responsa a las acciones del usuario como por ejemplo darle click a un botón, pasar el cursos, llenar fomularios, entre otros. Por lo tanto, para añadir controladores a los eventos del DOM se utiliza el addEventListener() para asignar una función a un elemento del DOM.

7. Describir al menos tres métodos para seleccionar elementos del DOM en JavaScript.

R//:

Métodos para seleccionar elementos DOM:

- getElementById(): este método selecciona un elemento por su ID.
- querySelector(): este método permite seleccionar un elemento utilizando un selector CSS.
- getElementsByClassName(): este método permite seleccionar un elemento por clase

8. ¿Cómo se crea un nuevo elemento HTML y se agrega al DOM utilizando JavaScript?

R//:
Se crea un nuevo elemento con document.createElement(), luego se puede configurar atributos y estilos (textContent)luego utilizando el método appendChild() se agrega el nuevo elemento al documento. 

9. ¿Cuál es la importancia de la manipulación del DOM en la creación de aplicaciones web dinámicas e interactivas?

R//:
La manipulación del DOM es esencial para crear aplicaciones web interactivas y dinámicas porque permite modificar el contenido de la página en tiempo real, un mejor dinamismo, adaptarse a diferentes dispositivos y responder a las acciones del usuario. Esto propende por una mejor experiencia para el usuario al tener una amplia gama de posibilidades con las interfaces al ser más atractivas y funcionales. 

10. Explicar brevemente los conceptos “event bubbling” y “event delegation” en el contexto de eventos del DOM. 

R//:

- Event Bubbling:
Es un fenómeno donde un evento se propaga desde el elemento específico hacia arriba en la jerarquía de padres.

- Event Delegation:
En términos de eventos, se entiende como, en lugar de poner un controlador de eventos en cada elemento, se pone un solo controlador en un elemento padre compartido. Es decir, cuando ocurre un evento en uno de sus hijos, el evento sube y es manejado por uno de sus padres.

11. ¿Por qué son relevantes los conceptos “event bubbling” y “event delegation” en la gestión de eventos en páginas web con múltiples elementos interactivos?

R//:
Esto dos conceptos simplifican y optimizan la gestión de eventos en páginas web con una serie de elementos interactivos y así, mejorando el código, posibilitando el manejo de elementos dinámicos y con un mejor mantenimiento y organización. 

*MÓDULO SOBRE COMUNICACIÓN CON EL SERVIDOR (STORAGE, PROMESAS,ASINCRONÍAS Y PETICIONES HTTPS)*

# Preguntas teóricas: 

1. Definir brevemente el concepto de localStorage y sessionStorage.

R//:
- LocalStorage: a grandes rasgos, es un espacio para almacenar información sin fecha de caducidad hasta que el usuario los elimine. 

- SessionStorage: a grandes rasgos, es un espacio para almacenar información pero de uso temporal.

2. Describir las diferencias claves entre localStorage y sessionStorage.

R//:
Una de las diferencias entre estos dos conceptos es que localStorage almacena datos incluso cerrando el navegador, mientras que por otras parte, sessionStorage al momentos de cerrar el navegador, se eliminan los datos.
Otra diferencias es que localStorage tiene un alcance globla, mientras que sessionStorage tiene un alcance limitado, es decir, en la pestaña que se creó.

3. ¿Por qué son útiles para almacenar datos en el navegador y cuál es su límite de capacidad?

R//:
Ambos, localStorage y sessionStorage son útiles para almancenar datos e información en el navegador del lado del usuario.
El límite	de capacidad está entre 5 MB y 10 MB, a veces depende del navegador que se utilice.  

4. ¿Qué son las promesas en JavaScript y para qué se utilizan en el desarrollo web?

R//:
Las promesas en JavaScript son una forma de manejar operaciones asincrónicas de unas maneras más clara y legible. Las promesas son un objeto que representa la eventual finalización (éxito o fallo) de una operación asincrónica y la devolución de su resultado. Las promesas tienen 3 estados posibles: Pendiente (Pending), Cumplida(Fulfilled) y Rechazada (Rejected).

5. Explica el concepto de asincronía en programación y cómo las promesas ayudan a manejar operaciones asincrónicas.

R//:
El concepto de asincronía hace alusión a la capacidad de ejecutar tareas independientes sin tener que esperar que cada tarea se ejecute para seguir con el flujo, es decir, el programa continúa su ejecución mientras que por otra parte las tareas asincrónicas en la cola se van procesando en segundo plano.

6. Proporciona un ejemplo de cómo se utiliza una promesa para realizar una operación asincrónica, como una solicitud de red.

R//: Ejemplo de una operación asincrónica. Ejemplo tomado de internet: 

function operacionAsincronica() {
  return new Promise((resolve, reject) => {
    setTimeout(() => {
      resolve('La operación asincrónica ha sido exitosa');
    }, 2000);
  });
}

7. ¿Qué es JSON Server y cómo se utiliza en el desarrollo web?

R//:
El JSON Server es muy útil para crear un modelo sin un backend real. Es muy necesario para hacer simulaciones con peticiones HTTP (GET, POST, PUT, DELETE) lo que facilita pruebas antes de tener un backend funcional.

8. ¿Por qué es útil simular una API REST falsa con JSON Server en el desarrollo frontend?

R//:
Simular una API REST falsa con JSON Server permite con antelación hacer pruebas, integraciones, depuraciones y esto agiliza el proceso de prototipado para posteriormente pasarla a un backend real o a un entorno de mayor producción. 

9. ¿Cuáles son las diferencias claves entre los métodos del objeto promesa .then().catch() y las palabras claves async/await?

R//:
Los métodos del objeto promesa .then().catch() es una forma tradicional de trabajar con promesas mientras que async/await proporciona una sintaxis más clara y fácil de entender para el código asíncrono.

10. Proporciona un ejemplo de cómo configurar una API falsa con JSON Server y realizar solicitudes (GET, POST, PUT, PATCH y DELETE) a través de ella.

R//:
Para configurar una API falsa con JSON Server se debe hacer lo siguiente: 

- Instalación de JSON Server:

npm install -g json-server

- Crear un archivo JSON en una carpeta por lo general llamada db.json: 

{
  "posts": [
    { "id": 1, "title": "Post 1" },
    { "id": 2, "title": "Post 2" }
    { "id": 3, "title": "Post 3" }
    { "id": 4, "title": "Post 4" }
  ]
}

- Se ejecuta JSON server (db.json):

json-server --watch db.json

- Realizar las solicitudes: 
(Ejemplo tomado de internet)

Ejemplo de solicitud GET
fetch('http://localhost:3000/posts')
  .then(response => response.json())
  .then(data => console.log('GET - Posts:', data))
  .catch(error => console.error('Error en GET:', error));

Ejemplo de solicitud POST
fetch('http://localhost:3000/posts', {
  method: 'POST',
  headers: {
    'Content-Type': 'application/json'
  },
  body: JSON.stringify({ title: 'Nuevo Post' })
})
  .then(response => response.json())
  .then(data => console.log('POST - Nuevo Post:', data))
  .catch(error => console.error('Error en POST:', error));

Ejemplo de solicitud PUT (actualización completa)
fetch('http://localhost:3000/posts/1', {
  method: 'PUT',
  headers: {
    'Content-Type': 'application/json'
  },
  body: JSON.stringify({ id: 1, title: 'Post Modificado' })
})
  .then(response => response.json())
  .then(data => console.log('PUT - Post Modificado:', data))
  .catch(error => console.error('Error en PUT:', error));

Ejemplo de solicitud PATCH (actualización parcial)
fetch('http://localhost:3000/posts/2', {
  method: 'PATCH',
  headers: {
    'Content-Type': 'application/json'
  },
  body: JSON.stringify({ title: 'Post Actualizado' })
})
  .then(response => response.json())
  .then(data => console.log('PATCH - Post Actualizado:', data))
  .catch(error => console.error('Error en PATCH:', error));

Ejemplo de solicitud DELETE
fetch('http://localhost:3000/posts/1', {
  method: 'DELETE'
})
  .then(response => console.log('DELETE - Post eliminado:', response.status === 200 ? 'Éxito' : 'Error'))
  .catch(error => console.error('Error en DELETE:', error));

11. Describe las diferencias entre Fetch y Axios como métodos para realizar solicitudes HTTP en JavaScript.

R//:
- Fetch: 
 Es una API nativa de JavaScript
 Su forma estandar de hacer solicitudes HTTP posibilita no recurrir a otras bibliotecas externas
 Utiliza una sintaxis más simple
 Está disponible en la mayoría de los navegadores modernos

- Axios:
Es una biblioteca de terceros
No está dentro del estándar de Javascript por lo que debe ser instalada
Es más intuitiva y con mejor facilidad a la hora de usar
Compatible con una amplia variedad de navegadores y de hecho algunos antiguos
Tiene un manejo de errores más sencillo y claro.

12. ¿Por qué es importante considerar las peticiones HTTP en aplicaciones web modernas?

R//:
Considerar las peticiones HTTP en aplicaciones web es muy necesario, puesto que siendo la comunicación entre el cliente y el servidor proveé de una diversidad de ventajas, como por ejemplo intercambio de datos, implementación de operaciones asíncronas, transmisión de información en tiempo real, intercambio de datos y construcción de APIS bien estructuradas, entre otras y todo esto para el óptimo desempeño de las aplicaciones web.

13. Proporciona ejemplos de cómo se utilizan Fetch y Axios para realizar solicitudes GET y POST.

R//:
Fetch:

GET con Fetch

fetch('https://jsonplaceholder.typicode.com/posts')
  .then(response => response.json())
  .then(data => console.log('GET - Datos:', data))
  .catch(error => console.error('Error en GET:', error));

POST con Fetch:

POST con Fetch
const postData = {
  title: 'Nuevo Post',
  body: 'Contenido del nuevo post',
  userId: 1
};

fetch('https://jsonplaceholder.typicode.com/posts', {
  method: 'POST',
  headers: {
    'Content-Type': 'application/json'
  },
  body: JSON.stringify(postData)
})
  .then(response => response.json())
  .then(data => console.log('POST - Nuevo Post:', data))
  .catch(error => console.error('Error en POST:', error));

Axios:

Primero se intala Axios:
- npm install axios

GET con Axios:

const axios = require('axios');

axios.get('https://jsonplaceholder.typicode.com/posts')
  .then(response => console.log('GET - Datos:', response.data))
  .catch(error => console.error('Error en GET:', error));

POST con Axios:

const axios = require('axios');

const postData = {
  title: 'Nuevo Post',
  body: 'Contenido del nuevo post',
  userId: 1
};

axios.post('https://jsonplaceholder.typicode.com/posts', postData)
  .then(response => console.log('POST - Nuevo Post:', response.data))
  .catch(error => console.error('Error en POST:', error));

14. Explica la importancia del manejo de errores al trabajar con promesas en el desarrollo web.

R//:
La importancia del manejo de errores al trabajar con promesas en el desarrollo web es: 
- Permite de manera adecuada manejar los errores y darles una correción.
- Brinda mayor información al usario sobre los posibles errores
- Proporciona seguridad, ya que al darle un bueno manejo a los errores evita posibles filtraciones de información.
- Facilita una mejor experiencia al usuario.

15. Describe cómo se manejan los errores en las promesas, incluyendo el uso de catch.

R//:

El manejo de errores en las promesas se realiza través de dos métodos: catch() y el segundo argumento de then(). El uso adecuado de los dos, permite una mejor funcionalidad de la aplicación y un óptimo manejo en los errores de las promesas dando como resultado una mejor confiabilidad.

catch(): 
este método captura cualquier error que haya ocurrido en las promesas anteriores a la cadena.

 then(): 
 se utiliza para manejar errores de manera específica de esa promesa.

16. ¿Cuáles son las diferencias claves entre los métodos del objeto promesa .then().catch() y la estructura try/catch?

R//:
Por un lado .then().catch() en particular se basa en el manejo de errores de las promesas, entre tanto, try/catch se comporta como una estructura más general al manejar errores en bloques de código, como síncronos y asíncronos, de tal forma, proporciona un control más amplio sobre los errores. 

17. Proporciona un ejemplo de cómo se puede manejar un error en una promesa al realizar una solicitud de red.

R//:
Ejemplo tomado de internet:

axios.get('https://api.pokemon.com/datos')
  .then(response => {
    console.log('Datos recibidos:', response.data);
  })
  .catch(error => {
    if (error.response) {
      console.error('Error en la respuesta:', error.response.status);
    } else if (error.request) {
      console.error('No se recibió respuesta del servidor');
    } else {
      console.error('Error al realizar la solicitud:', error.message);
    }
  });
 