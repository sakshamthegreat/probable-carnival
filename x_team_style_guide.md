# X-Team 01 Style Guide

**Style Guides**
Should be brief but sensible. Style guides are helpful in setting the standard for commenting in our group.

## Naming conventions

 **Variables**
* First character is never capitalized
* Variable names should give a general indicate idea as to what the variable will do
* Shouldn't be too long, but must be descriptive enough

 **Methods**
* First character is never capitalized
* Should be descriptive, more than variables
* Use underscores for spaces only in testing methods

 **Classes**
* First character is always capitalized
* Should only be a few words

 **Constants**
* Should be in all captials
* Space with underscores

### Examples
* interfaces

  public class testClass _implements interface_
  
* classes

  public class ExampleClass{
  
* exception types

   method throws Exception{
   
* fields

   public static final int CONSTANT_NAME = 20;
   
* methods

   public boolean exampleMethod(){
      return null;
   }
   
* parameters

  public boolean exampleMethod(_int example1, double example2_){
  
* local variables

    int localVariable = 0;
    
* instance constants

     private final int CONSTANT_NAME = 10;
     
* class constants

     public static final int CONSTANT_NAME = 20;
     
## Commenting style for public and private members of a class or interface:

Public and private members should be commented clearly without being excessive. For example, your roommate should be able to read your comments and understand what a program will do.

### Examples

* classes
Should specify the data structure used within the class, if any.

//This class uses an AVL tree.
public class BalancedSearchTree<T extends Comparable<T>> implements SearchTreeADT<T> { }

* fields
  (In many scenarios we will leave out comments for global fields - their names should be self-explanatory.)
  
  //freezing point for water in fahrenheit
  public static final int FAHRENHEIT_WATER_FREEZE_TEMP = 32;
  
* constructors
  
  public ClassName(){
  }
  
* methods
 /*
 * This method serves these purposes.
 * @param - this is a parameter argument
 * @throws - this exception
 * Known Bugs: this method has this bug in it
 /
 public int readThis(String text) throws IllegalArgumentException{
 }
 
* coding style (brackets, horizontal, and vertical spacing) for:
  * if statements
  
      if(exampleVariable == 5){
      }
  
  * switch statement
   
    switch (variableName) {
            case 1:  var = "0";
                     break;
            case 2:  var = "1";
                     break;
            case 3:  var = "2";
                     break;
            default: var = "10";
                     break;
    }
     
  * while loops
  
  while(exampleVariable == 0){
  }
  
  * for loops
  
  for(int a = 0; a < 2; a++){
      a = 3;
  }
  
  * enhanced for loops
  
   for(String element : array) {
    System.out.println("Element: " + element);
   }
