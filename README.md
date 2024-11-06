# Tecnologías elegidas

Elegí Node.js y Express porque son tecnologías que no uso actualmente, pero que quiero aprender. Además, considero que son ideales para esta actividad ya que permiten crear servicios HTTP de forma rápida y sencilla.

# Ejercicio seleccionado
El ejercicio consiste en exponer un servicio HTTP que determine si una palabra es palíndromo, es decir, si se lee igual de izquierda a derecha que de derecha a izquierda.

# Instrucciones para realizar las pruebas

1. Construir la imagen Docker:
 - Abrir terminal
 - docker buildx build . -t palindromo:1.0
 - docker run -p 8080:8080 palindromo:1.0

2. Al tener corriendo nuestro contenedor vamos a ver un mensaje en el que nos menciona que
 - El servidor esta corriendo en http://localhost:8080

3. Abrir el browser y utilizar esta url por ejemplo http://localhost:8080/palindromo?palabra=radar
 - La misma nos retornara un json del siguiente estilo
 - {"palabraRecibida":"radar","esPalindromo":true,"mensaje":"La palabra es un palíndromo."}
 - Se puede realizar diferentes pruebas cambiando el parametro palabra={miVariable}