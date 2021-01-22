import java.io.*;
import java.util.*;
class Employee
{
String name, address;
int age;
double salary;
double phnumber;
Employee(String n, String add, int a, double ph, double sa)
{
name = n;
address = add;
age = a;
phnumber = ph;
salary = sa;
}
void printSalary()
{
System.out.println("Salary= "+salary);
}
}
class Officer extends Employee
{
String specialization;
Officer(String n, String add, int a, double ph, double sa)
{
super(n, add, a, ph, sa);
}
}
class Manager extends Employee
{
String department;
Manager(String n, String add, int a, double ph, double sa)
{
super(n, add, a, ph, sa);
}
}
public class Main
{
public static void main(String args[])
{
Employee O1 = new Officer("Harry", "California", 20, 12345, 2000);
Employee M1 = new Manager("Mathew", "Mexico", 30, 98765, 2750);
System.out.println("Officer name is "+O1.name);
System.out.println("Officer address is "+O1.address);
System.out.println("Officer age is "+O1.age);
System.out.println("Officer phone number is "+O1.phnumber);
System.out.println("Officer salary is "+O1.salary);
System.out.println();
System.out.println("Manager name is "+M1.name);
System.out.println("Manager address is "+M1.address);
System.out.println("Manager age is "+M1.age);
System.out.println("Manager phone number is "+M1.phnumber);
System.out.println("Manager salary is "+M1.salary);
}
}

