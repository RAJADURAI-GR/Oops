import java.util.*; 
 class Ams
 { 
static public void main(String [] args) 
{ 
int s=0;
 Scanner s=new Scanner(System.in); 
System.out.println("Enter the number"); 
int n=s.nextInt();
 int k=n; 
while(n>0) 
{
 s=s+(n%10)*(n%10)*(n%10); 
n/=10; 
} 
if(k==s) 
System.out.println("The given number "+k+" is an armstrong number"); 
else 
System.out.println("The given number "+k+" is not an armstrong number"); 
}
}
#include <stdio.h>

#include <conio.h>

void create();

void insert();

void search();

void deletion();

void display();

int i, e, n, pos;

static int b[50];

main()

{

int ch;

char g'y';

create();

do

{

printf("\n List Operations");

printf("\n 1.Deletion\n 2. Insert\n 3. Search\n

4.Exit\n");

printf ("Enter your choice: ");

scanf("%d", &ch);

switch(ch)

{

case 1:

deletion();

break;

case 2:

insert();

break;

case 3:

search();

break;

case 4:

exit(0);

default:

printf("\n Enter the correct choice:");

} printf ("Do you want to continue: ");

fflush(stdin);

scanf("\n %c", &g);

} while (g=='y' || g=='Y');

getch();

2
}

void create()

{

printf("\n Enter the number of elements:");

scanf("%d",&n);

printf("\n Enter list elements: ");

for(i=0; i<n; i++)

scanf("%d", &b[i]);

}

void deletion()

{ printf("\n enter the position you want to delete: ");

scanf("%d", &pos);

if (pos >= n)

printf("\n Invalid location");

else

{

for (i=pos+1; i<n; i++)

b[i-1] n--: b[i]; printf ("List elements after deletion");

display();

}

}

void search()

{

int flag = 0;

printf("\n Enter the element to be searched: ");

scanf("%d", &e);

for(i=0; i<n; i++)

{

if (b[i] e) {

flag = 1; printf ("Element is in the ad position", i);

break;

}

} printf("Value &d is not in the list", e);

if (flag == 0)

}

void insert()

{

printf("\n Enter the position you need to insert: ");

scanf("%d", &pos);

if (pos >= n)

printf("\n Invalid location");

else

3
__________________________________________
2...

public class Main {

  public static void main(String[] args) {

    // value a, b, and c
    double a = 2.3, b = 4, c = 5.6;
    double root1, root2;

    // calculate the discriminant (b2 - 4ac)
    double discriminant = b * b - 4 * a * c;

    // check if discriminant is greater than 0
    if (discriminant > 0) {

      // two real and distinct roots
      root1 = (-b + Math.sqrt(discriminant)) / (2 * a);
      root2 = (-b - Math.sqrt(discriminant)) / (2 * a);

      System.out.format("root1 = %.2f and root2 = %.2f", root1, root2);
    }

    // check if discriminant is equal to 0
    else if (discriminant == 0) {

      // two real and equal roots
      // discriminant is equal to 0
      // so -b + 0 == -b
      root1 = root2 = -b / (2 * a);
      System.out.format("root1 = root2 = %.2f;", root1);
    }

    // if discriminant is less than zero
    else {

      // roots are complex number and distinct
      double real = -b / (2 * a);
      double imaginary = Math.sqrt(-discriminant) / (2 * a);
      System.out.format("root1 = %.2f+%.2fi", real, imaginary);
      System.out.format("\nroot2 = %.2f-%.2fi", real, imaginary);
    }
  }
}

Output:

root1 = -0.87+1.30i and root2 = -0.87-1.30i

___________________________________________
3.....
import java.util.Scanner;

class Matrixmul
               {
 	public static void main(String args[])
 	           {
 	    int m, n, p, q, sum = 0, i, j, k;
    Scanner in = new Scanner(System.in);

    System.out.println("Enter the number of rows and columns of first matrix");
m = in.nextInt();
n = in.nextInt();
         int first[][] = new int[m][n];

    System.out.println("Enter elements of first matrix");
 for (i = 0; i < m; i++)
 for (j = 0; j < n; j++)
first[i][j] = in.nextInt();

    System.out.println("Enter the number of rows and columns of second matrix");
p = in.nextInt();
q = in.nextInt();

    if (n != p)
System.out.println("The matrices can't be multiplied with each other.");

    else
      {
 int second[][] = new int[p][q];
 int multiply[][] = new int[m][q];
 System.out.println("Enter elements of second matrix");
 
 for (i = 0; i < p; i++)
 for (j = 0; j < q; j++)
second[i][j] = in.nextInt();

 for (i = 0; i < m; i++) 
 	     {
     for (j = 0; j < q; j++) 
          {
       for (k = 0; k < p; k++)
  sum = sum + first[i][k]*second[k][j];
             multiply[i][j] = sum;
         sum = 0;
}
 }

 System.out.println("Product of the matrices:");
 for (i = 0; i < m; i++) 
{
     for (j = 0; j < q; j++)
 System.out.print(multiply[i][j]+"\t");
    System.out.print("\n");
 }
      }
   }
}

_____________________________________________
4........
class Student
{ 
int id; 
String name;
 } 
class TestStudent3
{
 public static void main(String args[])
{
Student s1=new Student(); 
Student s2=new Student();
s1.id=101; 
s1.name="Sonoo";
 s2.id=102; s2.name="Amit"; 
System.out.println(s1.id+" "+s1.name); 
System.out.println(s2.id+" "+s2.name); 
}
}

____________________________________________
5.......
import java.io.*;
import java.lang.*;

   class StringOperation
       {
public static void main(String args[])
{
String s1="Hello";
String s2="World";

System.out.println("The strings are "+s1+" and "+s2);
int len1=s1.length();
int len2=s2.length();
System.out.println("The length of "+s1+" is :"+len1); 
System.out.println("The length of "+s2+" is :"+len2);
System.out.println("The concatenation of two strings = "+s1.concat(s2));
System.out.println("First character of "+s1+"is="+s1.charAt(0));
System.out.println("The uppercase of "+s1+"is="+s1.toUpperCase());
System.out.println("The lower case of "+s2+"is="+s2.toLowerCase());
System.out.println(" the letter e occurs at position " + s1.indexOf("e") + " in "+s1);
System.out.println("Substring of "+s1+"starting from index 2 and ending at 4 is = "+s1.substring(2,4));
System.out.println("Replacing 'e' with 'o' in "+s1+"is ="+s1.replace('e','o'));
System.out.println("The value of s1 = "+String.valueOf(s1));
boolean check = s1.equals(s2);

if(check==false)
System.out.println(""+s1+" and "+s2+" are not same"); 
else
System.out.println("" +s1+" and " +s2+" are same");
}
}
_____________________________________________6.......
import java.io.*;
 class alpha
 {
 public static void main(String args[]) 
{ 
String name[]={"Madras","Delhi","Ahameabad","Calcutta","Bombay"}; 
int size=name.length; String temp=null; 
int i,j; System.out.println("Before sorting:"); 
for(i=0;i<size;i++) 
for(j=i+1;j < size;j++)
if(name[j].compareTo(name[i])
{
temp=name[i]; 
name[i]=name[j]; 
name[j]=temp; 
} 
System.out.println("After sorting:"); 
for( i=0;i<size;i++)
{ 
System.out.println(name[i]);
 } 
}
 }







OUTPUT: 
C:\jdk1.3\bin>javac alpha.java 
C:\jdk1.3\bin>java alpha 
Before sorting: 
Madras
 Delhi 
Ahameabad 
Calcutta 
Bombay 
After sorting: 
Ahameabad 
Bombay 
Calcutta 
Delhi 
Madras
_____________________________________________7......
import java.util.Scanner;

 class Stud
       {
 String name;
 int regno;
 String dept;
 int mark[]=new int[5];
 int tot=0,avg;
}

class Student extends Stud
{
    void GetData() 						// Defining GetData()
        {
 	 Scanner in = new Scanner(System.in);

 System.out.print("\n\tEnter Student Name : ");
 name = in.next();

 System.out.print("\n\tEnter Student Reg. No. : ");
 regno = in.nextInt();

 System.out.print("\n\tEnter Department: ");
 dept = in.next();

 System.out.print("\n\tEnter the Marks :");

 for(int i=0;i<6;i++)
  {
 System.out.print("\n\tEnter Mark["+ (i+1) +"] : ");
 mark[i]=in.nextInt();
 tot+=mark[i];
 avg=tot/6;
 
 if(avg>=80)
        System.out.print("A");
        
 else if(avg>=60 && avg<80)
        System.out.print("B");
 
 else if(avg>=40 && avg<60)
 	   System.out.print("C");
        
 else
 	   System.out.print("D");
        
 }
}


     void PutData() 						// Defining PutData()
 	       {
        System.out.print("\n\n\t" +name + "\t" + regno + "\t\t" + dept + "\t" + tot + "\t" + avg +”\t” Grade);
                       }
           }

    class Stud_Inherit
         {
 public static void main(String args[])
 {
     Scanner in=new Scanner(System.in);

System.out.print("\n\nEnter the no. of Students: ");
int n=in.nextInt();

 Student[] obj = new Student[n];		// Array of Objects


 int i;
 for(i=0;i<n;i++)
 obj[i] = new Student(); 		// Allocating memory to each object

      for(i=0;i<n;i++)
         {
 System.out.print("\nEnter the details of "+ (i+1) +" Student\n");

 obj[i].GetData();
 }

 System.out.print("\nDetails of Students\n");
System.out.print("\n---------------------------------------------------------------");
System.out.println("\n\tName\tReg. No.\tDept.\tTotal\tAverage");
System.out.print("\n---------------------------------------------------------------");

 for(i=0;i<n;i++)
			obj[i].PutData();
 }
 }
_____________________________________________
8........

