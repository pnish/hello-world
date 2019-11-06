# hello-world

import java.util.*;
public class Main
{

    public static void main(String[] args) {    
            
      Scanner sc = new Scanner(System.in);
        String word = sc.next();   
        StringBuffer newstr = new StringBuffer(word);
            
        for(int i = 0; i < word.length(); i++) {    
                
            //Checks for lower case character    
            if(Character.isLowerCase(word.charAt(i))) {    
                //Convert it into upper case using toUpperCase() function    
                newstr.setCharAt(i, Character.toUpperCase(word.charAt(i)));    
            }    
            //Checks for upper case character    
            else if(Character.isUpperCase(word.charAt(i))) {    
                //Convert it into upper case using toLowerCase() function    
                newstr.setCharAt(i, Character.toLowerCase(word.charAt(i)));    
            }    
        }    
        System.out.println("String after case conversion : " + newstr);    
    }    
}
