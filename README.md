# Parcial-Funcional
# Criaderos de pollos

Tenemos un sistema que se ocupa de monitorear el alimento y salud de los pollos de criadero.

Un criadero tiene muchos pollos. De cada uno de ellos se conoce su peso (un número entero), su estado de salud (booleano que indica si está sano) y una descripción (una cadena de caracteres).

1) Se necesita alimentar a los pollos que requieran alimento y obtener cómo quedan todos los pollos (tanto los que se alimentaron como los que no). Un pollo require alimento si pesa menos de 1000 y alimentarlo consiste en aumentar su peso en un 10%
Hacer la función alimentar, no olvidar definir su tipo, y mostrar ejemplo de consulta y respuesta
 
2) Existen algunos medicamentos habilitados para pollos, lo que les provoca diferentes consecuencias: según qué medicamento sea. 
 a) una vacuna los deja con buena salud, y hace que su peso quede en 1000 unidades
 b) el antibiótico también los deja con buena salud, y aumenta su peso en tantas unidades como la el doble de la dosis que se utilice de dicho antibiótico
 c) hay unas pastillitas de colores que no alteran el peso ni la salud, pero se agrega el color de la pastilla al principio de la descripción del pollo. 

Los responsables de suministrar estos medicamento son los veterinarios. Hay varios, y cada uno se especializa en un medicamento (o eventualmente en varios que se suministran juntos) Cuando un veterinario hace su trabajo, le suministra a todos los pollos del criadero el medicamento en el que se especializa. 

Por ejemplo:
juan y pedro se especializan en vacunas
ana suministran un antibiotico con dosis 5, paula tambien pero con 10 de dosis.
tati se encarga de una pastilla verde
susana aplica una vacuna y a continuación una pastilla azul.
hay un veterinario bot que da placebos (que no le hacen nada a los pollos)
está tambien tatiana, que hace el trabajo de tati y de ana.

Hacer la función trabajar, que hace que un veterinario realice su trabajo en un criadero y permite obtener cómo quedan todos los pollos. 
Definir los veterinarios enumerados como ejemplo (y las funciones que sean necesarias para ello) y mostrar ejemplos de consulta con cada uno.

data Veterinario = UnVeterinario {
nombre:: String,
especialidad:: Pollo -> Pollo
}

3) Justificar la utilización de aplicación parcial y composición en la solución, señalando donde fueron utilizados y explicando qué ventajas tienen.
