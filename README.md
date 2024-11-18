# Frases Clásicas - Aplicación de Películas y Series 🎥✨  

¡Bienvenidos! Este repositorio contiene un proyecto diseñado para fortalecer tus habilidades en el desarrollo backend utilizando **Java**, **Spring Boot** y **bases de datos relacionales**. En esta aplicación, nos enfocamos en frases icónicas de películas y series, que se presentan de manera **aleatoria** en una interfaz intuitiva.

---

## Descripción del Proyecto 📜  

La aplicación muestra frases clásicas de películas y series, incluyendo información relevante como:  
- **Póster** de la película o serie.  
- **Título** de la obra.  
- **Frase destacada**.  
- **Personaje** que dijo la frase.  

Ejemplo de frases:  
- *"Amigos no mienten"* - Eleven (*Stranger Things*).  
- *"Yo no estoy en peligro, yo soy el peligro"* - Walter White (*Breaking Bad*).  
- *"¡Que la fuerza te acompañe!"* - Obi-Wan Kenobi (*Star Wars*).  
<p align="center">

  <img src="https://github.com/arcesoftware/screenmatch-frases/blob/main/picture.png"  style="margin:auto;">
</p>
Todas las frases y detalles se almacenan en una **base de datos local** configurada mediante **PG Admin** y manipulada con herramientas de consulta SQL.

---

## Objetivos del Proyecto 🚀  

1. **Practicar el uso de Spring Boot** para crear aplicaciones backend robustas.  
2. Desarrollar habilidades en el diseño y manejo de bases de datos relacionales.  
3. Conectar el backend con el frontend mediante **endpoints** REST.  
4. Implementar funcionalidades de consulta aleatoria para mejorar la experiencia del usuario.  

---

## Estructura del Proyecto 🗂️  

El proyecto se divide en los siguientes componentes principales:  

1. **Backend (Spring Boot):**  
   - Configuración del proyecto con **Spring Initializer**.  
   - Creación de endpoints para interactuar con los datos.  
   - Lógica para seleccionar frases de manera aleatoria.  

2. **Base de Datos (PostgreSQL):**  
   - Base de datos configurada con **PG Admin**.  
   - Población inicial de datos usando un script SQL.  

3. **Frontend:**  
   - Interfaz que muestra las frases y permite obtener nuevas frases aleatorias mediante un botón interactivo.  

---

## Configuración Inicial ⚙️  

### Prerrequisitos  
- [Java 17+](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)  
- [Maven](https://maven.apache.org/)  
- [Spring Boot](https://spring.io/projects/spring-boot)  
- [PostgreSQL](https://www.postgresql.org/) y [PG Admin](https://www.pgadmin.org/)  

### Pasos  
1. **Clona el repositorio:**  
   ```bash  
   git clone https://github.com/tu-usuario/frases-clasicas.git  
   cd frases-clasicas  


2. **Configura la base de datos:**

Abre **PG Admin** y crea una base de datos llamada frases.
Utiliza el **Query Tool** para ejecutar el script inicial de inserción de datos (disponible más abajo).

3. **Ejecuta la aplicación:**
   ```bash
   mvn spring-boot:run

4. **Accede al frontend:** 
  Abre un navegador y ve a http://localhost:8080

###Población de la Base de Datos 💾
Utiliza el siguiente script en **PG Admin** para insertar frases iniciales:
 ```bash
insert into frases(id, frase, personaje, titulo, poster) values (1, 'Amigos no mienten', 'Eleven', 'Stranger Things', 'https://m.media-amazon.com/images/M/MV5BMDZkYmVhNjMtNWU4MC00MDQxLWE3MjYtZGMzZWI1ZjhlOWJmXkEyXkFqcGdeQXVyMTkxNjUyNQ@@._V1_SX300.jpg');  
insert into frases(id, frase, personaje, titulo, poster) values (2, 'Bienvenida al mundo real. Es una droga. Te va a encantar', 'Monica', 'Friends', 'https://m.media-amazon.com/images/M/MV5BNDVkYjU0MzctMWRmZi00NTkxLTgwZWEtOWVhYjZlYjllYmU4XkEyXkFqcGdeQXVyNTA4NzY1MzY@._V1_SX300.jpg');  
