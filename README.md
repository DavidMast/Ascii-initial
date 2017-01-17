# My first programm

----
## Introduction
see [ascii art generator](http://patorjk.com/software/taag/#p=display&f=Big&t=Type%20Something%20)

> The aim of this first programm was to display our first name and last name initials. This programm introduced us the variables, the loop and the notions of class, interfaces and packages.

----
## How to install
We used Eclipse softare

----
## Packages

### ascii.big package

*contains BigInterface,
public class Big,the class corresponding to the letters initial public class D and M.*

>code example of the class Big

    package ascii.big;

    import ascii.AbstractFont;
    import font.CaracterInterface;

    public class Big extends AbstractFont implements BigInterface

----
### ascii package

*contains FontInterface,
public class Ascii,the public abstract class AbstractFont and AbstractCaracter.*

>code example of the class Ascii allowing to display the initials

    
       /*
        * Render lignes
        */
       for (int i = 0; i < font.getLineHeight(); i++) {

           /*
            * Render letters
            */
           for(int j = 0; j < caracterCollection.length; j++) {

               char [][] definition = caracterCollection[j].toAscii();
               /*
                * Render letters symbols
                */
               for (int k = 0; k < definition[i].length; k++) {
                

                   System.out.print(definition[i][k]);
                   
                }; 
                
           };
           
           System.out.println("");
           
       };


----
### font package

*contains FontInterface, CaracterInterface
and the public abstract class AbstractCaracter.*

>code example of the CaracterInterface

    
       package font;

       public interface CaracterInterface {
	
	       public String toString();
	       public char [][] toAscii();

       }

----
## Author
* myself

----
## thanks
* The teacher [Cyril Itchi] (https://www.linkedin.com/in/developer-php-cyril-ichti?authType=name&authToken=4HAF&trk=mirror-profile-memberlist-name)
