# Area-of-a-House-Calculator
* This program calculates the area of a house based on the inputs from the user. 

package simplecalculation;
import java.util.Scanner;
/**
 *
 * @author Max Peterson
 */
public class SimpleCalculation {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
    double length, width,height;
    double numDoors,wDoors,hDoors, numWindows, wWindows,hWindows,totalSurfArea, actualSurfArea;
    Scanner in = new Scanner(System.in);
    System.out.println("Please enter the length, width and height of the house?");
    length = in.nextDouble();
    width = in.nextDouble();
    height = in.nextDouble();
    totalSurfArea = (width * height * 2)+(length * height *2);
    System.out.println("How many doors does the house have?");
    numDoors = in.nextDouble();
    System.out.println("What is the width and height of the doors?");
    wDoors = in.nextDouble();
    hDoors = in.nextDouble ();
    System.out.println("How many windows does the house have?");
    numWindows = in.nextDouble ();
    System.out.println("What is the width and height of the windows?"); 
    wWindows = in.nextDouble();
    hWindows = in.nextDouble ();
    actualSurfArea = (totalSurfArea - (numDoors * wDoors * hDoors + numWindows * hWindows * wWindows));
    System.out.println("The total surface that needs to be painted is " + actualSurfArea);
    }

   
}
