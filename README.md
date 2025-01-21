# Oops
concepts related to Oops

/*public class Oops {

    public static void main(String args[]){
        Pen p1=new Pen();  //Creating pen object in memory
        p1.setcolor("Blue");
        p1.settip(5);
        System.out.println(p1.color);
        System.out.println(p1.tip);

    }
    
}
class Pen{

    String color;
    int tip;

    void setcolor(String newcolor){
        color=newcolor;
    }
    void settip(int newtip){
        tip=newtip;
    }
}

//Acess modifiers  1.private 2.default  3.protected    4.public
public class Oops{
    public static void main(String args[]){

        Bankaccount b1=new Bankaccount();
        b1.username="sourabh";
     b1.setpassword("GOOGLE");//we can only change the password cant change it

     System.out.println(b1.username);
     // System.out.println(b1.password); no acess
    }

}

class Bankaccount{

    String username;
   private String password;

    public void setpassword(String newpass){
        password=newpass;
    }


}

// Constructor overloading

public class Oops{
    public static void main(String args[]){
        Student s1=new Student();
        Student s1=new Student("sourabh");

    }
}

  class Student{
    String name;
    int roll;

    Student(){
      System.out.println("hello");

    }

    Student(String name){

        this.name="name";
    }
         
    }

    //Inheritance:
    import java.io.*;
    public class Oops{

        public static void main(String args[]){
          Fish f1=new Fish();
          f1.eat();
          f1.swim();  
          
          Mamamels M1=new Mamamels();
          M1.walk();
          M1.eat();
          M1.swim();
        }
    }
        class Animals{
            void eat(){
                System.out.println("animal eats");
            }
        }

        class Fish extends Animals{
            int fins;
            void swim(){
                System.out.println("fish swims");
            }

        }

        class Mamamels extends Fish{
              int legs;
              void walk(){
                System.out.println("mamels walk");
              }
        }
    
    //Mthod overloading(Same function name different parameters)

    import java.util.*;
    public class Oops{
        public static void main(String args[]){
            Calculator c1=new Calculator();
            System.out.println(c1.sum(1,2));
            System.out.println(c1.sum((float)1.5,(float)2.5,(float)4.0));

        }
    }
    class Calculator{

        int sum(int a,int b){
        return a+b;
    }

    float sum(float a,float b,float c){
        return a+b+c;
    }
}

//Method overriding concept(parent and child class has same function but diffferent def.)

import java.util.*;
public class Oops{
    public static void main(String args[]){
        Deer d1=new Deer();
        d1.eat();


    }
}
    class Animal{
        void eat(){
            System.out.println("eats anything");
        }
    }
    class Deer extends Animal{

        void eat(){
            System.out.println("eats grass");
        }
    } 

    //abstarct classes and methods(can't make object only make constructor)

    public class Oops{
    public static void main(String args[]){

        Horse h1=new Horse();
        h1.eat();
        h1.walk();

        Chicken c1=new Chicken();
        c1.eat();
        c1.walk();

    }
}

abstract class Animal {

    String color;

    Animal(){

        color="brown";
    }
    void eat(){
        System.out.println("eats food");
    }

    abstract void walk();
}

class Horse extends Animal{

    void changecolor(){
        color="dark brown";
    }

    void walk(){
        System.out.println("walks on two legs");
    }
}

class Chicken extends Animal{

    void walk(){
        System.out.println("walks on two legs");
    }
}

        //Interface

public class Oops{

    public static void main(String args[]){

        Bird b1=new Bird();
         b1.eats();
         b1.walk();


    }
}

 interface Animal {
             void walk();
             void eats();
}

class Bird implements Animal{

    public void walk(){
        System.out.println("Walks on two legs");
    }
    public void eats(){
        System.out.println("eats insects");
    }
}

//static keyword

   public class Oops{

    public static void main(String args[]){
        Student s1=new Student();
        s1.schoolname="MPEC";
        Student s2=new Student();
       // System.out.println(s2.schoolname);
        Student s3=new Student();
        s3.schoolname="MIPS";
System.out.println(s1.schoolname);//it will print MIPS because of the change & static key
    }
   }

   class Student{

    String name;
    int rollno;

    static String schoolname;

    void setname(String name){
        this.name=name;
    }

    String getname(){
        return this.name;
    }
   }
    */

    //super keyword  ("Calls the Parent constructor")

    public class Oops{

        public static void main(String args[]){
            Horse h1=new Horse();

        }
    }
    class Animal{

          Animal(){
            System.out.println("Animal constructor is called");
        }
    }

    class Horse extends Animal{
           Horse(){
            super();
            System.out.println("Horse class constructor is called");
        }
    }




    



