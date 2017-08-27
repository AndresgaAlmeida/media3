#Media3

Este exercício foi o segundo aprendido na aula de Programação Orientada a Objetos em Java. Ele mostra a importancia da aplicação do Método em um programa,
usando os recursos da P.O.O.
Com essa estrutura de controle de Fluxo podemos refinar ainda mais o programa



     import java.util.Scanner;

     public class Media3 {

              public static void main (String[] args){
     
     // Declarações
              Scanner teclado = new Scanner (System.in);
              float nota1, nota2, nota3, media;

    
    //  Leitura das notas
              
	      System.out.println("Informe as notas: ");
     
    // Nota 1:
    System.out.print("\n\tNota 1: ");
    nota1 = teclado.nextFloat();
    // Nota 2:
    System.out.print("\t Nota 2:");
    nota2 = teclado.nextFloat();
    // Nota 3:
    System.out.print("\t Nota 3: ");
    nota3 = teclado.nextFloat();
     
    
    //Calcula usando o método com retorno:
    media = calculaMedia (nota1, nota2, nota3);
    System.out.println("\n\tA média é " + media);

}  // Nesta chaves fechei o Main


    // O método estático (static) permite ser invocado sem a instancia da classe: public static float calculaMedia(float n1, float n2, float n3) {

        
         float media;

	 // Verifica as duas maiores notas e tira a média:
	 if (n1 < n2 && n1 < n3){   
	     media = (n2 + n3) / 2;
	 } else if (n2 < n3) {
             media = (n1 + n3) / 2;
	 } else {
	     media = (n1 + n2) / 2;
	 }
	 return media;
	 } 	
	 }
