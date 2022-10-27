Metodos
========================

**Filter**: se utiliza para eliminar elementos en base a un criterio. Devuelve un nuevo Stream por lo que podemos utilizar 
                otras operaciones aplicables a cualquier stream.
                
                   **Ejemplo:** cuenta la cantidad de valores del stream que comienzan con A o retornan true.
                   
    long cont = Stream.of("Claudia", "Alejandro", "Laika", "mama", "papa", "meme", "mimi").
    filter(predicado -> {
        predicado.startsWith("A");
        return true;
    }).count();
    System.out.println("CANTIDAD DE NOMBRES QUE EMPIEZAN CON A en el segundo stream: " + cont);
                
**Map**nos permite realizar una transformación rápida de los datos y muy directa sobre el flujo original.

   **Ejemplo:** imprime en mayuscula los valores del stream que comienzan con A
                
    Stream.of("Claudia", "Alejandro", "Laika", "mama", "papa", "meme", "mimi")
    .filter(predicado -> predicado.endsWith("a")).map(predicado -> predicado.toUpperCase())
    .forEach(predicado -> System.out.println(predicado));

**Sorted** ordena

 **Ejemplo:** devuelve un stream en mayuscula de todos los valores que empiezan con a  
 
    list.stream().filter(predicate -> predicate.startsWith("a"))
    .sorted().map(predicate -> predicate.toUpperCase())
    .forEach(predicate -> System.out.println(predicate));

**Concat**: Crea un flujo concatenado perezosamente cuyos elementos son todos los elementos del primer flujo seguidos de todos los elementos del segundo flujo.

  **Ejemplo:** Recibe dos stream los concatena y devuelve un stream ordenado

    String[] arreglo = { "Claudia", "Alejandro", "AA" };
    List<String> list = Arrays.asList(arreglo);
    		
    var stream1=list.stream();
    var stream2= Stream.of("Ailyn", "Laura", "Maria", "Dignora", "Esmeregilda");
    Stream.concat(stream1,stream2).sorted().forEach(predicate-> System.out.println(predicate));

**AnyMatch:** Devuelve si algún elemento de este flujo coincide con el predicado proporcionado. 

**Ejemplo:** imprimir en mayuscula ordenardos los nombres que tienen a como primera letra

		String[] arreglo = { "Claudia", "Alejandro", "AA" };
		List<String> list = Arrays.asList(arreglo);
		
		var stream1=list.stream();
		var stream2= Stream.of("Ailyn", "Laura", "Maria", "Dignora", "Esmeregilda");
		Stream <String> concat=Stream.concat(stream1,stream2);
		
		boolean contiene=concat.anyMatch(predicate->predicate.equalsIgnoreCase("maria"));
		Assert.assertTrue(contiene);
		
**Collectors.toList()** devuelve una lista a partir de un stream.
		
		List<String> list=Stream.of("A", "B", "C", "D")
		.filter(predicado -> predicado.equalsIgnoreCase("A"))
		.collect(Collectors.toList());
		System.out.println(list.get(0));

**Distinct()**:devuelve todos los elementos del stream sin repetirse

    List<Integer> values= Arrays.asList(1,2,5,8,2,1,9,10,8);
    values.stream().distinct().forEach(predicate->System.out.println(predicate));