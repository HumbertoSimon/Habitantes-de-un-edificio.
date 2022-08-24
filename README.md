# Habitantes-de-un-edificio.
Se deberá realizar un programa que pida al usuario que introduzca el numero de habitantes de cada puerta del edificio.  El programa debe decir la puerta que más habitantes tiene todo el edificio.


import java.util.Scanner;


public class NewMain {

   
    public static void main(String[] args) {
      Scanner scanner=new Scanner(System.in);
      
      System.out.println("Mete el numero de cuartos");
      
      int cantidadnumeros= scanner.nextInt();
        
      int numeromenor=0; 
      int numeromayor=0;
        
      for(int i=0; i <cantidadnumeros; i++){
    System.out.println("digite el numero de personas del cuarto no. " + (i+1));
    int tmp=scanner.nextInt();
    if(i==0){
    numeromenor=tmp;
    numeromayor=tmp;
    }else if(tmp<numeromenor){
    numeromenor=tmp;
    }
    if(tmp>numeromayor){
    numeromayor=tmp;
    }
    }  
     
      System.out.println("El cuarto con mas personas contiene :" +numeromayor + " personas");
      System.out.println("Y el cuarto con menos personas contiene :" +numeromenor + " personas");
    }
    
}
