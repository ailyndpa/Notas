Crear Stream
========================

**Un stream puede crearse de muchas formas, por ejemplo:**

*Con las factorías Stream.empty o Stream.of:*

var stream1 = Stream.empty();

var stream2 = Stream.of("a", "b", "c");

*O a partir de un array ya existente con el método Arrays.stream:*

var numeros = new int[] {1, 2, 3};
var stream = Arrays.stream(numeros);

*O a partir de una colección ya existente con los métodos stream y parallelStream proporcionados por las propias colecciones:*

var cadenas = List.of("a", "b", "c");

var secuencial = cadenas.stream();

var paralelo = cadenas.parallelStream();