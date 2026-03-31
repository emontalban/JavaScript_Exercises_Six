---
icon: brackets-square
---

# Tipos de datos

JavaScript tiene varios tipos de datos básicos que permiten representar diferentes tipos de información.

1. Tipos de Datos Primitivos:
   *   **string** → Representa una cadena de caracteres y  debe de colocarse entre comillas simples (`' '`), dobles (`" "`) o comillas invertidas (`` ` ` ``).&#x20;

       &#x20; &#x20;

       ```javascript
       let lenguaje = "JavaScript";
       ```
   *   **number** → Representa números tanto enteros como de coma flotante (decimales).

       &#x20; &#x20;

       ```javascript
       let versionActual = 2023;
       let precioTotal = 85.69; 
       ```
   *   **boolean** → Representan valores lógicos (true o false).

       &#x20; &#x20;

       ```javascript
       let esPopular = true;    
       let esObsoleto = false;
       ```

       &#x20;&#x20;
   *   **undefined** → Es el valor predeterminado de una variable declarada que aun no se le ha asignado valor.

       &#x20; &#x20;

       ```javascript
       let proximoLenguaje;
       ```
   *   **Null** → Representa la ausencia de Valor.

       &#x20; &#x20;

       ```javascript
       let lenguajeFavorito = null
       ```
   *   **Symbol** → Representa un valor unico e inmutable de cualquier valor.

       &#x20; &#x20;

       ```javascript
       let simboloJS = Symbol("JavaScript");
       ```
   *   **BigInt** → Se usa para números enteros extremadamente grandes que el tipo _`number`_ no puede manejar con precisión.

       &#x20; &#x20;

       ```javascript
       let lineasCodigoJS = 9007199254740993n
       ```



2.  Tipos de Datos compuestos:

    *   **object** → se utilizan para almacenar colecciones de datos y entidades más complejas.

        &#x20; &#x20;

        ```javascript
        let python = {
            nombre: "Python",
            creador: "Guido van Rossum",
            anio: 1991,
            tipadoDinamico: true
        };
        ```
    *   **array** → es una estructura de datos que permite almacenar una colección de elementos en una sola variable.

        &#x20; &#x20;

        ```javascript
        let lenguajes = ["JavaScript", "Python", "Java", "C++", "Ruby"];
        ```

    &#x20;&#x20;

    *   **Funciones** → Aunque técnicamente son objetos , se consideran un tipo especial que puede ser invocado.

        &#x20; &#x20;

        ```javascript
        function saludar(lenguaje) {
            return `Hola, bienvenido al mundo de ${lenguaje}!`;
        }
        ```

        &#x20; &#x20;

<figure><img src=".gitbook/assets/Tipo de datos.png" alt=""><figcaption></figcaption></figure>

