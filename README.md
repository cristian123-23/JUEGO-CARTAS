# JUEGO-CARTAS
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Classes/Main.java to edit this template
 */
package juegocartas1;


 

public class Juegocartas1 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        class Carta{
        String nombre;
      String poder;
      public Carta (String nombre,String poder){
          this.nombre=nombre;
          this.poder=poder;
      }
      public String toString(){
          return "carta{"+"nombre='" + nombre + '\" + ",poder='" + poder + '\" +'}';
      }
     }
class Carta {
    ArrayList<Carta> mazo;
    public Carta{
     mazo=new ArrayList<>();
     
     mazo.add(new Carta("CARTA 1","PODER 1"));
     mazo.add(new Carta("CARTA 2","PODER 2")); 
     mazo.add(new Carta("CARTA 3","PODER 3"));
     
     
     //BARAJA DE CARTAS
     Collection.shuffle(mazo);
}
    public void jugar (){
        Scanner SC=new Scanner(System.in);
        System.out.println ("¡BIENVENIDO AL JUEGO!");
        
        //logica de el juego
        while (mazo.size()>0){
            System.out.println("PRECIONA ENTER PARA SACAR UNA CARTA");
            SC.nextLine();
            Carta Carta =mazo.remove(0);
            System.out.println("HAS SACADO LA CARTA:"+ Carta);
            System.out.println("PODER DE LA CARTA:"+ Carta.poder);
            
        }
        SC.out.println("¡FIN DE EL JUEGO!");
    }
}
public class Main{
    public static void main ([]args){
        JuegoCartas juego=new
                JuegoCartas();
        juego.jugar();
    }
    
}
