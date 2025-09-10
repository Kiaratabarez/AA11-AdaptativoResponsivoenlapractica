Actividad: Adaptativo vs Responsivo en la práctica
Objetivo

Que los estudiantes comprendan, a través de la experimentación, la diferencia entre diseño adaptativo (saltos fijos) y responsivo (fluido).

Parte 1 – Diseño Adaptativo

Usar el siguiente ejemplo Adaptativo 

<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<title>Ejemplo Adaptativo</title>
<style>
body { margin: 0; font-family: sans-serif; }
.caja { background: lightblue; padding: 20px; }

/* Versión móvil */
@media (max-width: 480px) {
.caja { background: lightgreen; font-size: 14px; }
}

/* Versión tablet */
@media (min-width: 481px) and (max-width: 768px) {
.caja { background: lightcoral; font-size: 18px; }
}

/* Versión desktop */
@media (min-width: 769px) {
.caja { background: lightblue; font-size: 22px; }
}
</style>
</head>
<body>
<div class="caja">Este es un diseño adaptativo</div>
</body>
</html>

Ejecutar el código y cambiar el tamaño de la ventana.
Identificar en qué puntos cambia el color y tamaño del texto.
Tarea:

Agregar un nuevo breakpoint para pantallas grandes (ej. más de 1200px).
Hacer que el texto se vuelva violeta y la fuente de 28px en ese rango.
Parte 2 – Diseño Responsivo

Usar el siguiente ejemplo Responsivo 

<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<title>Ejemplo Responsivo</title>
<style>
body { margin: 0; font-family: sans-serif; }
.caja {
background: lightseagreen;
padding: 5%;
font-size: 2vw; /* escala según el ancho de la ventana */
}
</style>
</head>
<body>
<div class="caja">Este es un diseño responsivo</div>
</body>
</html>

Ejecutar el código y achicar/agrandar la ventana.
Observar cómo el texto cambia sin saltos.
Tarea:

Agregar 3 cajas más (<div class="caja">) con distintos textos.
Usar flexbox para que:
En pantallas grandes estén en fila.
En pantallas chicas se apilen en columna.
Parte 3 – Reflexión personal

¿Qué diferencias notaron en la experiencia de usuario entre ambos diseños?
¿Qué ventajas y desventajas vieron en cada enfoque?
¿En qué casos reales aplicarían uno u otro?
