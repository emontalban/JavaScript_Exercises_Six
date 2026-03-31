---
icon: file-lines
---

# Funciones de String

JavaScript tiene muchas funciones (llamadas métodos) para manipular cadenas de texto. Depende de lo que necesites hacer en ese momento.

Sin embargo vamos a  centrarrnos en 3 de ellas.

1.  Para  buscar contenido o verificar contenido **`.includes()`**

    Esta función dice si una cadena de texto contiene otra especifica dentro de ella. Devuelve un valor booleano (true o false) dependiendo si la contiene o no. Es Fundamental par validaciones rápidas.



    &#x20;\- Sintaxis: `texto.includes(termino_a_buscar)`

    &#x20; &#x20;

    ```javascript
    let saludo = "Hola, bienvenido al curso de JavaScript";

    console.log(saludo.includes("JavaScript")); // Resultado: true
    console.log(saludo.includes("Python"));     // Resultado: false
    ```
2.  Para modificar o Limpiar: **`.replace()`**

    Esta función  te permite buscar una parte del texto y reemplazarla por otra nueva. Por defecto, solo reemplaza la primera coincidencia que encuentra.



    &#x20;\- Sintaxis: `texto.replace(lo_que_busco, el_reemplazo)` &#x20;



    ```javascript
    let textoOriginal = "Estoy aprendiendo Java. Java es muy complicado.";

    let textoNuevo = textoOriginal.replace("Java", "JavaScript");

    console.log(textoNuevo);
    // Resultado: "Estoy aprendiendo JavaScript. Java es muy complicado."
    // Nota: Solo reemplazó el primer "Java".
    ```
3.  Para Extraer una Parte: **`.slice()`**

    Esta función  te permite  extraer un  porción de una cadena de texto y devolverla como una nueva cadena, _sin modificar la original_. Tú indicas dónde empieza la extracción y (opcionalmente) dónde termina.

    * **Indice inicio**: La posición del primer carácter a incluir (empezando en 0).
    *   **Indice fin opcional**: La posición _antes_ de donde termina la extracción. El carácter en este índice NO se incluye.

        &#x20; &#x20;

        &#x20; \- Sintaxis: `texto.slice(indice_inicio, indice_fin_opcional)`&#x20;

        *   En JavaScript se puede contar los indices de dos formas:<br>

            1.  **Indices Positivos** (De izquierda a derecha): Empiezan en `0` para el primer carácter, `1` para el segundo, etc.



                ```javascript

                let frase = "JavaScript es un lenguaje de programacion.";
                // Índices:   0123456789...

                // Ejemplo 1: Extraer desde el índice 0 hasta *antes* del 10
                let palabra1 = frase.slice(0, 10);
                console.log(palabra1); // Resultado: "JavaScript"

                // Ejemplo 2: Extraer desde el índice 14 hasta el final
                let palabra2 = frase.slice(14);
                console.log(palabra2); // Resultado: "un lenguaje de programacion."
                ```
            2.  **Indices Negativos** (De derecha a izquierda): Empiezan en `-1` para el _último_ carácter, `-2` para el penúltimo, `-3` para el antepenúltimo, y así sucesivamente.\
                <br>

                ```javascript
                let frase = "JavaScript es un lenguaje de programacion.";
                // Índices:   0123456789...

                // Ejemplo 1: Extraer desde el índice -25 hasta el -17
                let palabra1 = frase.slice(-25 ,-17);
                console.log(palabra1); // Resultado: "lenguaje"

                // Ejemplo 2: Extraer desde el índice -13 hasta el final
                let palabra2 = frase.slice(-13);
                console.log(palabra2); // Resultado: "programacion."
                ```



<figure><img src=".gitbook/assets/Funciones String.png" alt=""><figcaption></figcaption></figure>
