# Practica-02-POO-con-Java
**Nombre: Franklin Orellana**

**Practica N° 2 Enlaces de Clases**

**Carrera: Computación**

# OBJETIVO ALCANZADO: 
- Como objetivo alcanzado fue tener un mejor conocimiento de objetos en java y a la vez tener aclarar el manejo de herencias entre varias 
clases en este caso de la clase abuelo a las clases padres y de las clases padre a las clases hijas.

- Se implemento downcasting, el instanceof y una lista para guardar datos e imprimirlos.

## 1.	Crear un repositorio en GitHub con el nombre “Práctica 02 – POO con Java”.

- Se creo un repositorio en GitHub con el nombre dado en la guia de Practica.

## 2.	Sincronizar el repositorio creado con un proyecto en NetBeans. Realizar un commit y push por cada requerimiento de los puntos a continuación descritos (incluir un mensaje que identifique claramente los commits realizados a GitHub).

- Se realizo 5 commits en el proyecto

## 3.	Crear un paquete para las clases, otro para las interfaces, otro para las pruebas

- Se crearon los 3 paquetes:

      - clases
      
      - interfaces
      
      - prueba
      
## 4. Crear una jerarquía de clases de tres niveles, es decir, una clase “abuelo”, dos clases “padres” y cuatro clases “hijas” (dos de cada padre).

-	Para la clase abuelo se le designo el nombre: “ Juego ”

-	Para las clases padres se les designo los nombres: “Juegos De Azar y Juegos Digitales”

-	Para las clases hijas se les designo los nombres: ” Aventura, Deporte, Póker, Bingo”

## 5.	Todas las clases deben tener por lo menos cuatros atributos (aparte de los de herencia), tres métodos (aparte de los getters y setters) y método toString().

      - Atributos, metodos y toString de la clase Juego
      
      public class Juego {
    
    /**
     * atributos de la clase Juegos
     */

    private int codigo;
    
    private String nombre;
    
    private String categorias;
    
    private int numeroJugadores;
    
    

