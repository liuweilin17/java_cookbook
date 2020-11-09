### Features

* JDK/JRE

  JDK, Java Development Kit, It includes the Java Runtime Environment (JRE), an interpreter/loader (Java), a compiler (javac), an archiver (jar), a documentation generator (Javadoc) and other tools needed in Java development.

  JRE, Java Runtime Environment, it provides the minimum requirements for executing a Java application; it consists of the *Java Virtual Machine (JVM), core classes*, and *supporting files*.

* static import

  In Java, static import concept is introduced in 1.5 version. With the help of static import, we can access the static members of a class directly without class name or any object. For Example: we always use sqrt() method of Math class by using Math class i.e. **Math.sqrt()**, but by using static import we can access sqrt() method directly.
  According to SUN microSystem, it will improve the code readability and enhance coding. But according to the programming experts, it will lead to confusion and not good for programming. If there is no specific requirement then we should **not** go for static import.

  ```java
  // Java Program to illustrate 
  // calling of predefined methods 
  // without static import 
  class Geeks { 
      public static void main(String[] args) 
      { 
          System.out.println(Math.sqrt(4)); 
          System.out.println(Math.pow(2, 2)); 
          System.out.println(Math.abs(6.3)); 
      } 
  } 
  ```

  ```java
  // Java Program to illustrate 
  // calling of predefined methods 
  // with static import 
  import static java.lang.Math.*; 
  class Test2 { 
      public static void main(String[] args) 
      { 
          System.out.println(sqrt(4)); 
          System.out.println(pow(2, 2)); 
          System.out.println(abs(6.3)); 
      } 
  } 
  ```


### DataType

* byte

  *Todo*

* Integer vs int

  *Todo*

* Optional

  *Todo*

* Stream

  *Todo* (InputStream, OutputStream)

### Function

* Lambda

  *Todo*

### OOD

* Interface

   ```java
   // Create an instance with implemented interface
   Interface1 instance1 = new Interface1();
   {
     @Override
     public void method1(){return "method1";}
   }
   ```

   
