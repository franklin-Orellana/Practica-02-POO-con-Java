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
    
    
  /**  
   * metodos clase abuelo
   */
   
    
    public void partidaInicio(){
        System.out.println(""+this.nombre);
    }
    
    public void partidaTerminada(){
        System.out.println(""+this.nombre);
    }
    
    /**
     * generacion de toString de la clase Juegos 
     */
    
    @Override
    public String toString() {
        return "n\t\tJuego" + "\nCodigo: " + codigo + "\nNombre: " + nombre + "\nCategorias: " + categorias + "\nNumero De Jugadores: " + numeroJugadores + '"';
    }
    
    - Atributos, metodos y toString de la clase JuegosDeAzar
    
     /**
     * atributos de la clase JuegosDeAzar
     */
    
    private int numeroMesa;
    private boolean fisico;
    private String nombreDealer;
    private String nombreJuego;
    
    /**
     * metodos de la clase padre 
     */
    
    public void cambioMesa(){
    }
    
    public void cambiomodoJuego(){ 
    }
    
    public void cambionombreDealer(){
        
    }
    
    /**
     * generacion de toString de la clase JuegosDeAzar 
     */
     
    @Override
    public String toString() {
       return super.toString() + "\n\t\tJuegos De Azar" + "\nNumero de Mesa: " + numeroMesa + "\nFisico: " + fisico + "\nNombre del Dealer: " + nombreDealer + "\nNombre de Juego: " + nombreJuego + '"';
    }
    
    - Atributos, metodos y toString de la clase JuegosDigital
    
     /**
     * atributos de la clase JuegosDigitales
     */
    
    private boolean modoOnline;
    private boolean digital;
    private String plataforma;
    private String graficos;

    /**
     * metodos de la clase padre 
     */
    
    
    public void cambioPlataforma() {
    }

    public void cambiomodoOnline() {
    }
    
    /**
     * generacion de toString de la clase JuegosDigital
     */
    
    @Override
    public String toString() {
        return super.toString() + "\n\t\tJuegos Digitales" + "\nOnline: " + modoOnline + "\nDigital: " + digital + "\nPlataforma: " + plataforma + "\nGraficos: " + graficos + '"';
    }

    
    - Atributos, metodos y toString de la clase Aventura
    
    /**
     * atributos de la clase Aventura
     */
    
    private String misiones;
    private String objetivos;
    private String logro;
    private String mapa;
    
    /**
     * metodos de la clase aventura 
     */

    public void guardarMisiones(){
    }
    
    public void guardarMapa(){
    }
    
    public void guardarLogros(){
    }
    
    /**
     * generacion de toString de la clase Aventura
     */
    
    @Override
    public String toString() {
        return super.toString() + "\nAventura" + "\nmisiones: " + misiones + "\nobjetivos: " + objetivos + "\nlogro: " + logro + "\nmapa: " + mapa + '"';
    }
    
    - Atributos, metodos y toString de la clase Deporte
    
    /**
     * atributos de la clase Deporte
     */
    
    private String nombreEquipo;
    private String tiempo;
    private boolean cambioJugador;
    private boolean cambioTactica;
    
    /**
     * metodos de la clase aventura 
     */
    
    public void cambiarnombreEquipo(){
    }
    
    public void modificarTiempo(){
    }
    
    public void modificarTactica(){
    }
    
    /**
     * generacion de toString de la clase Deporte
     */
    
    @Override
    public String toString() {
        return super.toString() + "\n\t\tDeporte\n" + "\nNombre De Equipo: " + nombreEquipo + "\nTiempo De Juego: " + tiempo + "\nCambio De Jugador: " + cambioJugador + "\nCambio De Tactica: " + cambioTactica + '"';
    }
    
    - Atributos, metodos y toString de la clase Bingo
    
    /**
     * atributos de la clase Bingo
     */
    
    private int numeroTabla;
    private int numeroBolas;
    private String tipoPremio;
    private boolean comprobarTabla;
    
    /**
     * metodos de la clase bingo 
     */

    public void cambiarTabla(){
    }
    
    public void cambiartipoPremio(){
    }
    
    public void modificarnumeroBolas(){
    }
    
    /**
     * generacion de toString de la clase Bigo
     */
    
    @Override
    public String toString() {
        return super.toString() + "\n\t\tBingo" + "\nnumeroTabla: " + numeroTabla + "\nnumeroBolas: " + numeroBolas + "\ntipoPremio: " + tipoPremio + "\ncomprobarTabla: " + comprobarTabla + '"';
    }
    
    - Atributos, metodos y toString de la clase Poker
    
    /**
     * atributos de la clase Poker
     */

    private int tipoFicha;
    private int numeroPuesto;
    private double apuesta;
    private String mostrarJuegos;
    
    /**
     * metodos de la clase poker 
     */
    
    public void cambiartipoFicha(){
    }
    
    public void modificarApuesta(){
    }
    
    public void cambiarnumeroPuesto(){
    }
    
    /**
     * generacion de toString de la clase poker
     */
    
    @Override
    public String toString() {
        return super.toString() + "\n\t\tPoker" + "\nTipo de Ficha: " + tipoFicha + "\nNumero de Puesto: " + numeroPuesto + "\nApuesta: " + apuesta + "\nMostrar Juegos: " + mostrarJuegos + '"';
    }
    
    
## 6.	Cada clase padre debe tener por lo menos un método abstracto cada una.

-	Método abstracto de la clase padre JuegosDigitales


    /**
     * metodo abstracto de la clase padre
     */
     

    public abstract void Multijugador();

-	Método abstracto de la clase padre JurgosDeAzar


    /**
     * metodo abstracto de la clase padre
     */


    public abstract void Reglas ();
  
  
##7. Los métodos abstractos deben ser sobre-escritos (implementados) en cada clase hija.

      ##- Clase Aventura
      
      
    /**
     * metodos abstracto implementadoaa la clase Aventura
     */
    
    @Override
    public void Multijugador() {
        System.out.println("El juego es multijugador y pueden jugar hasta "+this.getNumeroJugadores()+" jugadores");    
    }

    @Override
    public void partidaInicio() {
        System.out.println("Partida a dado inicio " +this.getNombre());    
    }

    @Override
    public void partidaTerminada() {
        System.out.println("La Partida a terminado " +this.getNombre());    
    }
      
      ##- Clase Deporte
      
      
    /**
     * metodos abstracto implementadoaa la clase Deporte
     */
    
    @Override
    public void Multijugador() {
        System.out.println("El juego es multijugador y pueden jugar hasta "+this.getNumeroJugadores()+" jugadores");    
    }

    @Override
    public void partidaInicio() {
        System.out.println("La Partida a dado inicio " +this.getNombre());    
    }

    @Override
    public void partidaTerminada() {
        System.out.println("La Partida a terminado "+ this.getNombre());    
    }
            
      ##- Clase Póker
      
      
    /**
     * metodos abstracto implementadoaa la clase Poker
     */
    
    @Override
    public void Reglas() {
        System.out.println("En el "+this.getNombre()+" no es permitido mostrar las cartas a otro oponente");
    }

    @Override
    public void partidaInicio() {
        System.out.println("Partida a dado inicio "+this.getNombre());    
    }

    @Override
    public void partidaTerminada() {
        System.out.println("La Partida a terminado "+this.getNombre());
    }
      
      
      ##- Clase Bingo
      
    /**
     * metodos abstracto implementadoaa la clase Bingo
     */
    
    
    @Override
    public void Reglas() {
        System.out.println("En el "+this.getNombre()+" no puede haber mas de dos fichas en el mismo casillero ");
    }

    @Override
    public void partidaInicio() {
        System.out.println("Partida a dado inicio "+this.getNombre());
    }

    @Override
    public void partidaTerminada() {
        System.out.println("La Partida a terminado "+this.getNombre());
    }
    
    



