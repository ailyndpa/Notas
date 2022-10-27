Trabajo con arreglos
========================

**Para declarar un arreglo en este caso es de entero para un espacio en memoria de 5 valores***
		String [] array= new String[5];
		*Asignando valores*
		array[0]="zero";
		array[1]="one";
		array[2]="two";
		array[3]="three";
		array[4]="four";
		
System.out.println("El arreglo array en la posicion 0 tiene como valor: "+ array[0]);
		
**Otra manera de crear y asignar valores a un array**
		int [] array2= {5,6,7,8,9,10};
		
System.out.println("El arreglo array2 en la posicion 3 tiene como valor: "+array2[3]);
		
**loop** 
		System.out.println("Imprimiendo valores del arreglo array: ");
		for(int i=0; i<array.length;i++) {
			System.out.println(array[i]);
		}
		System.out.println("Imprimiendo valores del arreglo array2: ");
		
*otra manera con menos complicación*
		for(int valor: array2) {
			System.out.println(valor);	
		}
*Imprimir los valores pares del array2*
		System.out.println("Imprimiendo valores pares del arreglo array2: ");
		for(int valor: array2) {
			if(valor%2==0) {
				System.out.println(valor);
				//break; se usa para salir del ciclo una vez que encuentre un valor par
			}
		}
		
