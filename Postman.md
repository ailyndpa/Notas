Postman
=======

1- Descargar el poyecto del repositorio
2-Ubicarse en la carpeta donde lo descargo y abrir una consola de comandos
3- Instalar las dependencias, en este caso el proyecto es node y seria, npm install
4- cuando se hayan instalado todas las dependencias iniciar el proyecto, npm start
5-Buscar archivo readme para mejor información
6- Dirigirse a la carpeta routes y abrir el archivo index para ver las rutas que debe probar
7- a la url base se le adiciona la ruta para probar un servicio especifico

Para obtener un recurso por medio de la id existen dos formas:
1- {{urlBase}}/movies/:id
Se guarda automaticamente en la pestaña Params en una nueva sección la key: id y como valor el que se le especifique.

2-{{urlBase}}/movies/{{idMovie}}
y el valor de idMovie se guarda como variable  en la colección

**TEST1**
const response= pm.response.json();// Obtiene la respuesta en formato json
const varId= Object.keys(response).includes("id")// verifica que la respuesta incluya la key id
pm.test("Validate id", ()=>{
   pm.expect(true).to.be.equal(varId)
})

**TEST2**
const response= pm.response.json();// Obtiene la respuesta en formato json
const movieDrama=response.filter((movie)=>movie.genre==="Drama");// filtra por peliculas con genero Drama

movie=movieDrama[0]// Obtiene la primera prelicula drama
pm.test("Movie find for by genre", ()=>{
    pm.expect(movie).to.be.an('object');//verifica que movie sea un objeto
    pm.expect(movie.genre).to.eq('Drama')//verifica que el genero sea drama
})
**TEST3**

const movieSchema = {
    title: '',
    year: 0,
    genre: "",
    director: "",
    rate: 0
}
const body = JSON.parse(pm.request.body.raw);
const someSchema=JSON.stringify(Object.keys(movieSchema)) === JSON.stringify(Object.keys(body));
pm.test("Same schema", ()=>{
pm.expect(true).to.be.eql(someSchema);
})

**GUARDAR TOKEN ACTUALIZADO**
const res=pm.response.json();
pm.globals.set('token',res.accessToken);


jsonData = pm.response.json();

**GUARDA LAS KEYS EN GLOBAL**
jsonData = pm.response.json();
/** 
 * Save properties in global
 * */
const defaultKeys = ['title', 'year', 'genre', 'director', 'rate'];
/**
 * Extraer propiedades del response
 * if not response
 * else
 * defaul Value 
 * */
const keys = jsonData?.lenght > 0 ? Object.keys(jsonData[0]) : defaultKeys;

/**Asignar variables */
keys.map(key => pm.globals.set(key, (data[key] && data[key] != '') ? data[key] : (jsonData[0])[key]))



const params = pm.request.url.query.map(({key, value}) => ({
    key,
    value: (data[key] && data[key] != "" ) ? data[key]: value,
}))