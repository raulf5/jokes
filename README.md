# Briefing del Proyecto: Chistes 

## Descripción  
En entregas anteriores, los datos utilizados en nuestras webs se agregaban manualmente al programa (hardcoded), pero esto no es lo habitual.  

Al igual que en la mayoría de webs reales, consumiremos datos de una API en este ejercicio. Usaremos una API ya existente para obtener un listado de naves (chistes) fácilmente.  

Los temas principales que practicarás en este proyecto son:  
- **TypeScript**  
- **Obtención de datos mediante llamadas API Rest** a un servidor.  

### Contexto del Cliente  
Una empresa de coaching está realizando un experimento en empresas de Barcelona para medir el impacto del humor y la diversión en la productividad. Han solicitado una aplicación web que muestre chistes a los empleados antes de comenzar la jornada laboral.  

**Tu rol**: Serás responsable de desarrollar la base del proyecto para una demo en 2 semanas con el cliente y comenzar pruebas con usuarios reales.  

---

## Información Técnica  
### API a Consumir  
- **Documentación de la API**: [Calling the API](https://icanhazdadjoke.com/api)  
- **Endpoint para obtener un chiste aleatorio**: [Random dad joke](https://icanhazdadjoke.com/)  
- **Header necesario**:  
  ```  
  'Accept': 'application/json'  
  ```  

### Notas del Responsable Front End  
- **Obligatorio**:  
  - Implementar bucles y lógica con ES6 (usar `map`, `reduce`, `filter`, `sort`).  
  - **No se permite el uso de `for`**.  
  - Desarrollo en **TypeScript** (requisito común en entrevistas técnicas).  
- **Configuración inicial de TypeScript**:  
  [Pasos para preparar un proyecto TypeScript](https://www.digitalocean.com/community/tutorials/typescript-new-project).  

---

## Nivel 1  
### Ejercicio 1: Pantalla Principal  
- Al iniciar, mostrar el primer chiste y un botón "Siguiente chiste".  
- Al presionar el botón, hacer `fetch` a la API y mostrar el chiste en consola y pantalla.  

**Ayudas**:  
- Usar `Promises` o `async/await` para manejar la respuesta de la API.  
- Probar la API con Postman antes de implementarla.  

### Ejercicio 2: Maquetación Inicial  
- Maquetar la web colocando elementos básicos (chiste, botones).  
- Propuesta visual:  
  ![Ejemplo](https://itacademy.barcelonactiva.cat/pluginfile.php/29703/mod_assign/intro/exercici2.png)  

### Ejercicio 3: Seguimiento de Uso  
- Crear un array `reporteChistes` para almacenar:  
  ```typescript  
  {  
    joke: "...",  
    score: 1, // Rango: 1-3 (1 = peor)  
    date: "YYYY-MM-DDTHH:MM:SSZ" // Formato ISO  
  }  
  ```  
- Implementar 3 botones de puntuación.  
- Permitir cambiar la puntuación antes de pasar al siguiente chiste.  
- Mostrar el array actualizado por consola.  

---

## Nivel 2  
### Ejercicio 4: Integración Meteorológica  
- Consumir una API de información meteorológica y mostrar los datos al inicio de la app.  

### Ejercicio 5: Alternar APIs de Chistes  
- Integrar una segunda API de chistes (ej: Chuck Norris) para alternar fuentes.  

---

## Nivel 3  
### Ejercicio 6: Maquetación Avanzada  
- Maquetar la web siguiendo el diseño propuesto:  
  ![Diseño](https://itacademy.barcelonactiva.cat/pluginfile.php/29703/mod_assign/intro/exercici7.png)  
- Usar **SVG** para formas dinámicas (herramienta: [Blob Generator](http://magicpattern.design/tools/blob-generator)).  
- **Bonus**: Cambiar la forma del contenedor al cargar un nuevo chiste.  

---

## Objetivos  
- Entender el funcionamiento de APIs.  
- Explorar APIs gratuitas.  
- Implementar tests unitarios.  

### Duración: 4-5 días  
### Entrega:  
- URL del repositorio Git.  
