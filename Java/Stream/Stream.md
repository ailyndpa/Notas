Stream
========================

Introducida en Java 8, la API Stream se utiliza para procesar colecciones de objetos. Un stream es una secuencia de objetos que soporta varios métodos que pueden ser canalizados para producir el resultado deseado.

*Un stream no es una estructura de datos, sino que toma la entrada de las Colecciones, Arrays o canales de E/S.
*Los flujos no cambian la estructura de datos original, sólo proporcionan el resultado según los métodos canalizados.
*Cada operación intermedia se ejecuta perezosamente y devuelve un flujo como resultado, por lo que se pueden canalizar varias operaciones intermedias. Las operaciones terminales marcan el final del flujo y devuelven el resultado.