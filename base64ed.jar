/*
Program for encode text to base64 
or decode with java.util.base64;
*/
import java.lang.*;
import java.util.*;



public class base64ed {
    public static void main(String[] args) {
        //<--- create objects
        Scanner in = new Scanner(System.in);
        int EnterCommand;
        String EnterText;
        byte[] bytesDeEncode;

        WriteLn("Hello, it is base64 encode text \n 1: text to base64 \n 2: base64 to text \n 3: exit");
        EnterCommand = 0;
        while (EnterCommand != 3) {

            Write("cmd > ");

            //<--- it is get command for select next step
            EnterCommand = in.nextInt();

            switch (EnterCommand) {
                case 1: {
                    Write("cmd > encode > ");
                    Scanner in2 = new Scanner(System.in);
                    EnterText = in2.nextLine();
                    bytesDeEncode = Base64.getEncoder().encode(EnterText.getBytes());
                    WriteLn("Your encoded text: " + new String(bytesDeEncode));
                    break;
                }

                case 2: {
                    Write("cmd > encode > ");
                    Scanner in2 = new Scanner(System.in);
                    EnterText = in2.nextLine();
                    bytesDeEncode = Base64.getDecoder().decode(EnterText.getBytes());
                    WriteLn("Your decoded text: " + new String(bytesDeEncode));
                    break;
                }

                default: {
                    ///<--- for exit if command not=1,2,3
                     EnterCommand = 3;
                }

            }
        }

    }

    public static void WriteLn(String SText) {
        System.out.println(SText);
    }

    public static void Write(String SText) {
        System.out.print(SText);
    }
}
