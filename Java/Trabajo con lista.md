Trabajo con lista
============

ArrayList<String> lista=new ArrayList<String>();
		lista.add("Ailyn");
		lista.add("Geider");
		lista.add("blablabla");
		lista.add(0, "Odalys");
		
System.out.println("ArrayList "+lista);
System.out.println("valor 3 de la Lista "+lista.get(3));
		
for(String valor: lista) {
	System.out.println("valor= "+valor);
}
  *Imprimir Ailyn*
String nombreCompleto="Ailyn del Pino Acosta";
String[] arreglo=nombreCompleto.split(" ");
System.out.println(arreglo[0]);		
				
System.out.println("Imprimiendo el nombre completo en posicion vertical de alante hacia atras");
for(int i=0; i<nombreCompleto.length();i++) {
	System.out.println(nombreCompleto.charAt(i));
}

System.out.println("Imprimiendo el nombre completo en posicion vertical de atras hacia delante");
for(int i=nombreCompleto.length()-1; i>=0;i--) {
	System.out.println(nombreCompleto.charAt(i));
}