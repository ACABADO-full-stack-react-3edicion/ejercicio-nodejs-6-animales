# Ejercicio Node.js Animales

Crea una base de datos relacional con MySQL que refleje el siguiente modelo de datos:

- Existen dueños, que tienen una id numérica, un nombre, una edad, y un DNI (único).
- Existen animales, que tienen una id numérica, un nombre, una edad, una especie y un número de chip (único).
- Existen especies, que tienen una id numérica y un nombre (único).
- Cada animal pertenece a un solo dueño o a ninguno. Un dueño puede tener cero, uno o varios animales.

Crea una aplicación en Node.js que se conecte a la base de datos anterior, con las siguientes especificaciones.

- Primero se le debe preguntar al usuario su DNI. Si no existe en la base de datos, se muestra un mensaje diciéndolo y se acaba el programa.
- Luego se le dan una serie de opciones:
  · Listar todos mis animales
  · Listar todos mis animales de una especie
  · Mostrar los datos de uno de mis animales
  · Adoptar un animal
  · Cambiar mi nombre
- Si ha elegido "Listar todos mis animales", la aplicación debe listarle todos sus animales, ordenados por especie y por nombre.
- Si ha elegido "Listar todos mis animales de una especie", se le hará otra pregunta para que introduzca la especie (por nombre), y se listarán todos sus animales de esa especie, ordenados por especie y por nombre.
- Si ha elegido "Mostrar los datos de uno de mis animales", se le hará otra pregunta para que introduzca el número de chip, y luego se le mostrarán los datos del animal correspondiente (o un mensaje si no se encuentra el animal).
- Si ha elegido "Adoptar un animal", se le preguntará qué animal quiere adoptar, y se le darán como opciones a elegir (choices) todos los animales que no tienen dueño. Cuando elija uno, la aplicación debe modificar el animal en la base de datos para que tenga como dueño al usuario.
- Si ha elegido "Cambiar mi nombre", se le preguntará el nuevo nombre y la aplicación debe modificar su nombre en la base de datos.
