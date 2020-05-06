# Statiic-initializer
main() method without a code in it.

import java.util.Scanner;
public class Main
{

  static Scanner input = new Scanner (System.in);
  static{
      System.out.println("enter the breadth of the parllelogram");
  }
  static int B = input.nextInt ();
  static{
      System.out.println("enter the height of the parllelogram");
  }
  static int H = input.nextInt ();

  static
  {
    try
    {
     if (B <= 0 || H <= 0){throw new Exception ("Breadth and height must be positive");}
	    else{System.out.println("the area of parllelogram is "+B*H);}
    }
    catch (Exception e)
    {
      System.out.println (e);
    }

  }
  public static void main (String[]args){}
  			
}
