### Encapsulation in Java

Encapsulation is the mechanism in which data and functions that manipulate the data are bound together, and that keeps both safe from outside interference and misuse. In encapsulation the variables of a class will be hidden from other classes, and can be accessed only through the methods of their current class, which is also known as data hiding.

To achieve encapsulation in Java

* Declare the variables of a class as private.

* Provide public setter and getter methods to modify and view the variables values.

### For Example


```

/* File name : Student.java */
public class Student{

   private String name;
   private String idNum;
   private int age;

   public int getAge(){
      return age;
   }

   public String getName(){
      return name;
   }

   public String getIdNum(){
      return idNum;
   }

   public void setAge( int newAge){
      age = newAge;
   }

   public void setName(String newName){
      name = newName;
   }

   public void setIdNum( String newId){
      idNum = newId;
   }
}

```

### Getters & Setters

The public setXXX() and getXXX() methods are the access points of the instance variables of the Student class. Normally, these methods are referred as getters and setters. Therefore any class that wants to access the variables should access them through these getters and setters.

```

/* File name : RunStudent.java */
public class RunStudent{

   public static void main(String args[]){
      Student std = new Student();
      std.setName("Mary");
      std.setAge(20);
      std.setIdNum("39871");

      System.out.print("Name : " + std.getName() + " Age : " + std.getAge());
    }
}

```


### Benefits of Encapsulation:

* The fields of a class can be made read-only or write-only.

* A class can have total control over what is stored in its fields.

* The users of a class do not know how the class stores its data. A class can change the data type of a field and users of the class do not need to change any of their code.
