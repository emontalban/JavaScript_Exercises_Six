---
icon: question
---

# Operador Ternario

El operador ternario es un operador condicional de JavaScript que actúa como una forma compacta y abreviada de la instrucción `if...else`.\
\
Su sintaxis básica sigue el formato

```javascript
 condición ? expresión_verdadera : expresión_falsa.
```

El funcionamiento del operador se divide en tres partes fundamentales divididas por los símbolos `?` y `:`:

1. Condición: Una expresión que se evalúa como verdadera o falsa.
2. Expresión verdadera: El valor o acción que se retorna si la condición es _true_. `?` separa la condicion del resultado positivo
3. Expresión falsa: El valor o acción que se retorna si la condición es _false_. `:`Separa el resultado positivo del negativo.

El operador evalúa el punto de partida (la condición) y devuelve inmediatamente uno de los dos valores proporcionados, otorgando una gran versatilidad ya que puede devolver funciones, objetos, números o cadenas.<br>

Su uso principal es condensar lógica condicional compleja en una sola línea de código para que sea más elegante y eficiente. Entre sus aplicaciones más comunes se encuentran:

* Asignaciones condicicional: Guardar un valor en una variable basándose en una condición.
* Retorno de funciones: Permite simplificar funciones que solo necesitan devolver un resultado basado en una validación.
* Valores por defecto: Se utiliza frecuentemente para asignar valores predeterminados cuando una propiedad o variable no está definida.
* Dentro de plantillas de texto (Template Literals): Muy útil para insertar lógica dentro de un mensaje.
* En React y Frameworks Modernos: Se usa para decidir qué componente mostrar en la pantalla (renderizado condicional)

No es recomendable usarlo cuando:

* Tienes múltiples condiciones (`else if` anidados). Se vuelve muy difícil de leer.
* Las acciones que quieres ejecutar son bloques de código largos.

Con `if...else` tradicional:

```javascript
let edad = 20;
let mensaje;

if (edad >= 18) {
  mensaje = "Puedes pasar";
} else {
  mensaje = "No puedes pasar";
}
```

Con operador Ternario<br>

```javascript
let edad = 20;
let mensaje = (edad >= 18) ? "Puedes pasar" : "No puedes pasar";
```



<figure><img src=".gitbook/assets/Operador Ternario.png" alt=""><figcaption></figcaption></figure>
