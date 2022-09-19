- 👋 Hi, I’m @LucasRCTaborda
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
LucasRCTaborda/LucasRCTaborda is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->




/**
 * Escreva uma descrição da classe trabalhooo aqui.
 * 
 * Uma escola está interessada no uso do WhatsApp pelos alunos para fins educacionais. Para isso, ela entrevistou vários alunos e coletou os seguintes dados: idade, 
 * quantidade de grupos de estudo no WhatsApp que o aluno participa e tempo diário (estimado) em minutos que aluno usa (interage nos grupos) o WhatsApp para estudar.
 * Faça um programa que leia os dados necessários e informe (escreva na tela) o que a escola deseja saber: 

(a) Percentual de alunos que usam o WhatsApp por mais de uma hora ao dia para estudar. 

(b) Idade média dos alunos que usam o WhatsApp para estudar. 

(c) Maior tempo (em hora e minuto) gasto no WhatsApp por um aluno para estudar. 

(d) Idade do aluno que participa de mais grupos.

Defina uma condição de parada para que sejam informados dados de tantos alunos quantos o usuário do programa desejar.
 * @author (Lucas Taborda) 
 * @version (18/09)
 */
import java.util.Scanner;
public class trabalhooo
             {   public static void main(String args[]){ 
                 Scanner teclado = new Scanner (System.in) ;
    
         int idade=0,idademedia=0 ,grupo=0,tempodeuso=0,alunos=0,cont=0 ,a=0,b=0,c=0,d=0,gg=0 ;
         int v;
       
  System.out.printf("\f");
               do{
        System.out.println("deseja adicionar mais alunos na pesquisa se sim (1) senão (2)");
        v=teclado.nextInt();
         if( v==1 )  {
             
                
        do{  System.out.print("Escreva sua idade :  ");
                                   idade=teclado.nextInt();
                                   } while(idade<0 );  
                                   
           
       do{  System.out.print("Quantidade de grupos em qual participa:  ");
                                   grupo=teclado.nextInt();   
                                   }while(grupo<0); 
                                   
       do{  System.out.println("Tempo de uso em minutos :  ");
                                   tempodeuso=teclado.nextInt();    
                                } while (tempodeuso<0);        
             
               alunos++;
               idademedia=idademedia+idade;
               
         if(tempodeuso>c)c=tempodeuso;
         if(tempodeuso>60) cont++;
         if(grupo>gg) gg=grupo;
         if (grupo>=gg)d=idade;
         
            a=(cont*100/alunos); 
            b=(idademedia/alunos);    

if(tempodeuso<=0)System.out.println("Valor de negativo invalido ");}
 else if(v==2)System.out.println("Obrigado o resultado a seguir corresponde a pesquisa"); 


}while(v==1) ;
System.out.println("O percentual de alunos que usam mais de 1 hora para estudar  " +a+ "%");

System.out.println("A idade media dos alunos que usam o whatsapp para estudar  "+b);
    
System.out.println("O maior tempo gastos em hora e minuto para estudar  "+(c/60)+" hora e "+(c%60) +" Menutos");
    
System.out.println("a idade do aluno que participa de mais grupo  "+d); 
}
}
