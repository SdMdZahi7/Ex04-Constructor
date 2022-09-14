# Ex04-Constructor
## Aim:
 To write a C# program to calculate the salary of an employee by passing the name, designation, noofexperience, basic salary and insurance amount through constructor.
 
 ## Algorithm:
##Step1:
Start

##Step2:
Create a class and a constructor

##Step3:
Get name, designation, noofexperience, basic salary and insurance amount from the User.

##Step4:
call salary method in constructor to calculate salary.

##Step5:
call display method to display the output.

##Step6:
stop
 
 
 
 ## Program:
 ~~~
 using System;
using System.Security.Cryptography;

namespace Zahi
{
    public class program
    {
        static void Main(String[] args)
        {
            string name, desig;
            int exp, bs, ins, hra, ta, s;
            void salary(int bs, int ins)
            {

                hra = (20 * bs) / 100;
                ta = (10 * bs) / 100;
                s = bs + hra + ta - ins;
            }
            void display()
            {
                Console.WriteLine("Name of the employee is " + name + " having " + exp + " of experience, working as " + desig);
                Console.WriteLine("Receives " + s + " of salary");
            }

            Console.WriteLine("Enter name of the employee: ");
            name = Console.ReadLine();
            Console.WriteLine("Enter designation of the employee: ");
            desig = Console.ReadLine();
            Console.WriteLine("Enter years of experience of the employee: ");
            exp = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("Enter basic salary of the employee: ");
            bs = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("Enter insurance: ");
            ins = Convert.ToInt32(Console.ReadLine());
            salary(bs, ins);
            display();


        }
    }
}
~~~
 
 ## Output:
 ![CONSTRUCTOR 1](https://user-images.githubusercontent.com/94187572/190171597-8fe12107-3f3f-4859-ba66-582c34978f05.png)

 ## Result:
 Thus C# program to calculate the salary of an employee by passing the name, designation, noofexperience, basic salary and insurance amount through constructor is executed successfully.


