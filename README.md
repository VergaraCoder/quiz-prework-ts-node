# quiz-prework-ts-node
Test

Preguntas Abiertas (10)
JavaScript Básico:

Describe qué es una función en JavaScript y cómo se declara.
  -Una funcion es un bloque de intrucciones que ejecutan una pequeña funcionalidad y que todo en su declarado en su interior solo esta al cance de la misma

Manipulación del DOM:
Explica cómo seleccionar un elemento del DOM y cambiar su contenido.
  -Una forma sencilla de seleccionar un elemento puede ser con el metodo querySelector(".nombreClase") y tenemos bastantes mas y una forma rapida de cambiar su contenido con                   (elemento.textContent="nuevo valor")

Programación Orientada a Objetos (OOP):
¿Qué es una clase en JavaScript y cómo se define una?

  -Una clase en javascript es una representacion de un agente que tiene distintas propiedades como,peso,color etcc. pero ademas este agente puede tener cualidades unicas que se les denomina       metodos aunque en realidad son funciones dentro de la clase que le dan cierto comportamiento 
  DEFINICION DE UNA CLASE--> class nombre{}

    
Eventos en JavaScript:

¿Cómo se agrega un evento de clic a un botón en JavaScript?
Variables y Tipos de Datos:

  Se debe seleccionar el elemento y luego aplicar un addEventListener("click")
  const elemento=document.querySelector(".button");
  elemento.addEventListener("click",()=>{});
  

Explica las diferencias entre var, let, y const en JavaScript.

const--> variables que son fijas (osea no se puede cambiar su valor)
let --> Forma para declarar una varibale que mas adelante del codigo puedes cambiar su valor
var-> Tiene el mismo alcance (se le dice scope) que const

_______________________________________


Control de Flujo:
¿Qué son las estructuras de control de flujo y cuáles son algunas de las más comunes en JavaScript?

  La mas comun --> (if,else if,else)  
  otro un poco--> (switch,case,default)

_______________________________________


Funciones de Flecha:

Describe qué es una función de flecha en JavaScript y proporciona un ejemplo de cómo se usa.
  Una funcion flecha es un tipo de funcion que no me acuerdo en que version de javascript se implemento
  las funciones flechas tienen la siguinete sintaxis cuando se van a implementar de manera independiente--> const nameFunction=()=>{};

_______________________________________

  
JSON:
¿Qué es JSON y cómo se utiliza en JavaScript?

  JSON es un formato estandar para el envio de datos mas especificamente objetos.
  En javascript su uso es principalemente para la transferencia de objetos ,ya sea en localStorage etc..
  Este funciona junto con dos metodos principales , que son: 
  
    JSON.parse--> Esta forma transformamos los datos empaquetados en forma de string para convertilos a un objeto

    JSON.stringify--> Esta forma se utiliza para transformar un objeto a string para poder ser enviado 

_______________________________________


Promesas:
Explica qué es una promesa en JavaScript y proporciona un ejemplo de su uso.

  Una promesa se utiliza para operaciones que pueden requerir un poco de tiempo para ser ejecutadas como por ejemplo una peticion a una base de datos , o para que hayan otros procesos mientras 
  se realiza este proceso asincrono--> ejemplo

  const peticion=(URLbase)=>{
    return new Promise((req,res)=>{
      const request= fetch(URLbase+"/profiles");
      if(!request.ok){
        req("Algo salio mal");
      }

      res(request.json());
    });
  }


peticion(urlDirection)
.then((object)=>{
  console.log(object);
})
.catch((err)=>{
  console.log(err);
})
_______________________________________

Depuración:

¿Cuáles son algunas de las herramientas o métodos que se pueden usar para depurar código JavaScript?
Preguntas de Selección Múltiple (20)
¿Cuál de las siguientes es la forma correcta de declarar una variable en JavaScript?
A) var myVariable;  
B) variable myVariable;
C) let myVariable;
D) A y C son correctas. //CORRECTA
¿Qué método se utiliza para agregar un elemento al final de un array en JavaScript?
A) push() //CORRECTO
B) pop()
C) shift()
D) unshift()
¿Cuál de los siguientes operadores se utiliza para comparar tanto el valor como el tipo de dos variables en JavaScript?
A) ==
B) === //CORRECTO
C) !=
D) !==
¿Cuál es la salida del siguiente código?
console.log(typeof null);
A) null  
B) undefined //CORRECTO
C) object
D) number
¿Cuál de los siguientes métodos se usa para recorrer todos los elementos de un array?
A) forEach()
B) map()
C) filter()
D) Todas las anteriores //CORRECTO

¿Qué se entiende por “hoisting” en JavaScript?

A) Declaraciones de variables y funciones se mueven al principio de su ámbito.
B) Es un término para describir la eliminación de variables.
C) Es un método para agrupar varias funciones.
D) Ninguna de las anteriores.  //CORRECTO

¿Cuál es la diferencia entre null y undefined en JavaScript?
A) null significa que una variable ha sido declarada pero no definida, undefined significa que no se ha declarado.
B) null es un valor asignado intencionalmente, undefined significa que una variable no tiene valor. //CORRECTO
C) undefined es un valor asignado intencionalmente, null significa que una variable no tiene valor.
D) No hay diferencia.


¿Cuál es el propósito del método Array.prototype.map()?
A) Modificar el array original. //CORRECTO
B) Crear un nuevo array con los resultados de aplicar una función a cada elemento del array original.
C) Filtrar los elementos de un array.
D) Encontrar un elemento en un array.


¿Qué es el Event Loop en JavaScript?
A) Un ciclo que controla las llamadas recursivas.
B) Un proceso que permite a JavaScript realizar operaciones asincrónicas.
C) Un método para iterar sobre arrays.  //CORRECTO
D) Ninguna de las anteriores.


¿Cuál es la salida del siguiente código?

console.log(0.1 + 0.2 === 0.3);
A) true  //CORRECTO
B) false
C) undefined
D) NaN


¿Qué se entiende por strict mode en JavaScript?

A) Un modo que permite utilizar características experimentales.
B) Un modo que cambia la forma en que se ejecuta JavaScript, haciéndolo más seguro.
C) Un método para validar datos.
D) Ninguna de las anteriores.  //CORRECTO


¿Cuál de las siguientes es una forma correcta de crear un objeto en JavaScript?

A) let obj = {};
B) let obj = Object.create();
C) let obj = new Object();
D) A y C son correctas.  //CORRECTO


¿Qué es un callback en JavaScript?

A) Una función que se pasa como argumento a otra función. //CORRECTO
B) Un tipo de variable especial.
C) Un método para declarar funciones.
D) Ninguna de las anteriores.


¿Cuál es el propósito de async y await en JavaScript?

A) Ejecutar funciones síncronas.
B) Manejar operaciones asincrónicas de manera más simple y legible.  //CORRECTA
C) Declarar variables globales.
D) Ninguna de las anteriores.


¿Cuál de las siguientes es una estructura de datos inmutable en JavaScript?
A) Arrays
B) Strings
C) Objetos
D) Ninguna de las anteriores. //CORRECTA


¿Cómo se puede convertir un objeto JSON en una cadena de texto en JavaScript?
A) JSON.parse()
B) JSON.stringify() //CORRECTA
C) toString()
D) parseInt()


¿Qué es un Promise en JavaScript?
A) Una función que se ejecuta inmediatamente.
B) Un objeto que representa la eventual finalización (o falla) de una operación asincrónica. //CORRECTA
C) Un método para declarar variables.
D) Ninguna de las anteriores.


¿Qué método se utiliza para agregar uno o más elementos al principio de un array y devolver la nueva longitud del array?
A) push()
B) pop()
C) shift() //CORRECTA
D) unshift()


¿Cuál es la diferencia entre localStorage y sessionStorage en JavaScript?
A) localStorage almacena datos solo durante la sesión del navegador, sessionStorage almacena datos de manera persistente.
B) sessionStorage almacena datos solo durante la sesión del navegador, localStorage almacena datos de manera persistente. //CORRECTA
C) No hay diferencia entre ellos.
D) Ambos almacenan datos solo durante la sesión del navegador.


¿Qué método se utiliza para detener la propagación de un evento en el DOM?
A) event.stopPropagation() //CORRECTA
B) event.preventDefault()
C) event.stop()
D) event.cancel()
