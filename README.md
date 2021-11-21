# areaFinder
import java.util.Scanner;

abstract class shape {
    int width;
    abstract void area();
}
//your code goes here

 class square extends shape{
   public square(int widt){
        width=widt;
    }
    public void area(){
        System.out.println(width*width);

    }
}
 class circle extends shape {
    public circle(int wid){
        width=wid;
    }
    public void area(){
        System.out.println(Math.PI *width*width);

    
    }
}
public class Program {
    public static void main(String[ ] args) {
        Scanner sc = new Scanner(System.in);
        //System.out.println("eneter the width of square")
        int x = sc.nextInt();
        //System.out.println("enter the radius odf the")
        int y = sc.nextInt();
        
        square a = new square(x);
        circle b = new circle(y);
        //System.out.println(a.widt);
        a.area();
        b.area();
    }
}
