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

## Configuración de la Base de Datos  

### Pasos para configurar la base de datos:  

1. **Crea la base de datos:**  
   - Abre **PG Admin** y crea una base de datos llamada `frases`.  

2. **Ejecuta el script inicial:**  
   - Utiliza el **Query Tool** en PG Admin para ejecutar el script inicial de inserción de datos (disponible más abajo).  

## Ejecuta la Aplicación  
  ```bash 
  mvn spring-boot:run
 ```
---

## Acceso al Frontend  

- Abre un navegador y ve a: [http://localhost:8080](http://localhost:8080)  

---

## Población de la Base de Datos 💾  

Utiliza el siguiente script en **PG Admin** para insertar frases iniciales:  

```sql
insert into frases(id, frase, personaje, titulo, poster) values 
(1, 'Amigos no mienten', 'Eleven', 'Stranger Things', 'https://m.media-amazon.com/images/M/MV5BMDZkYmVhNjMtNWU4MC00MDQxLWE3MjYtZGMzZWI1ZjhlOWJmXkEyXkFqcGdeQXVyMTkxNjUyNQ@@._V1_SX300.jpg');

insert into frases(id, frase, personaje, titulo, poster) values 
(2, 'Bienvenida al mundo real. Es una droga. Te va a encantar', 'Monica', 'Friends', 'https://m.media-amazon.com/images/M/MV5BNDVkYjU0MzctMWRmZi00NTkxLTgwZWEtOWVhYjZlYjllYmU4XkEyXkFqcGdeQXVyNTA4NzY1MzY@._V1_SX300.jpg');
 ```
-- Agrega más registros según sea necesario.

## Agregar Nuevas Frases  

Sigue este formato para agregar nuevas frases:  

```sql
insert into frases(id, frase, personaje, titulo, poster) values (id, 'frase', 'personaje', 'título', 'poster');
 ```
## Obtén los Pósters desde el sitio OMDb API

- Busca el título en **inglés** y utiliza el enlace proporcionado en el **JSON devuelto** para asegurar la uniformidad de los tamaños de las imágenes.

### Ejemplo:

```sql
insert into frases(id, frase, personaje, titulo, poster) values 
(11, 'La vida pasa muy rápido. Si no nos detenemos para disfrutarla de vez en cuando, pasa y ni la ves!', 'Ferris Bueller', 'Viviendo la vida loca', 'https://m.media-amazon.com/images/M/MV5BMDA0NjZhZWUtNmI2NC00MmFjLTgwZDYtYzVjZmNhMDVmOTBkXkEyXkFqcGdeQXVyMTQxNzMzNDI@._V1_SX300.jpg');
 ```
## Contribuciones 🤝

¿Tienes una idea para mejorar el proyecto?  
¡Las contribuciones son bienvenidas!

- Abre un **Pull Request** o reporta un **Issue** en el repositorio.

---

## Licencia 📄

Este proyecto está bajo la licencia **MIT**.

---

¡Gracias por participar en este desafío! 🎉  
Diviértete explorando las frases clásicas y aprendiendo mientras desarrollas.  
¡Que la fuerza te acompañe! 🌟






