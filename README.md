# value-if-base-and-power-is-given-using-recursion-
recursion


import java.util.*;
import java.io.*;

public class HelloWorld{

     public static void main(String []args)
     {
         Scanner sc=new Scanner(System.in);
         int n=sc.nextInt();
         int pow=sc.nextInt();
         int res=check(n,pow);
         System.out.println(res);
     
     }
     static int check(int n,int pow)
     {
         if(pow==0)
         {
             return n;
         }
         return n*check(n,pow-1);
     }
}
