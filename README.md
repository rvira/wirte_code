Problem Statement: https://www.hackerrank.com/challenges/printing-pattern-2/problem

```
import java.util.Scanner;

public class test {
       public static void main(String[] args) {
           System.out.println("Enter n: ");
           Scanner sc = new Scanner(System.in);
           int n = sc.nextInt();
           for (int i = n; i >0; i--) {
               int j=n,k;
               for (k = 0; k < n; k++) {   
                 if(j<i){
                   j++;
                   System.out.print(j+" ");
                 }
                 else{
                   System.out.print(j+" ");
                 }
                 j-=1;
              }
               j=i;
               int flag = n-i-1;
               for (k=0; k < n-2; k++) {
                   
                 if(k>=i-1 && flag>0){
                     j++;
                     flag--;
                 } 
                 System.out.print(j+" ");
                   
              }
               System.out.print(n);
               System.out.println("");
           }
           
           for (int i = 1; i <n; i++) {
               
               int j=n,k;
               for (k = 0; k < n; k++) {   
                 if(j>i){
                   System.out.print(j+" ");
                 }
                 else{
                     j++;
                   System.out.print(j+" ");
                 }
                 j-=1;
              }
              j=i+1;
               int flag = n-i-1;
               for (k=0; k < n-2; k++) {
                   
                 if(k>=i && flag>0){
                     j++;
                     flag--;
                 } 
                 System.out.print(j+" ");
                   
             }
               System.out.print(n);
               System.out.println("");
           }
   }
}

```
