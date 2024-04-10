Title Codtech IT Solutiion - Task Documentation calculator with advance features,which implements a calculator with advanced features such as addition, subtraction, multiplication, division,exponentiation, and the option to quit.

Introduction this documantation provides a detailed explanation of the task assigned during the CODTECH IT solutions Intremship program.the task is writing a java program to calculator with advanced features such as addition, subtraction, multiplication, division,exponentiation, and the option to quit. 
This documentation will cover the implementation details, rationale behind the code structure, and insights into the programming techniques utilized.Additionally, it will include introduction about the interm Venkatesh Chedu and his assigned ID, ICOD6226.

Interm Information: Name: Venkatesh Chedu Interm ID: ICOD6226

Task Description:
The Task assigned to Venkatesh Chedu during the CodTech ITsolution internship program is to write a java program simple calculator with advance features,
which implements a simple calculator with advanced features such as addition, subtraction, multiplication, division,exponentiation, and the option to quit.

Implementation: 
the implementation of the task involves utilizing java program language to create a simple program that interates from calculator. 
The program uses "while" loop to achieve functionality efficienty. 

implementation Overview:
The Simple Calculator program is a Java application designed to perform basic arithmetic operations such as addition, subtraction, multiplication, division, and exponentiation.
It provides users with a menu-driven interface for selecting the desired operation and inputting two numbers to perform the calculation.
This documentation provides a detailed explanation of the code implementation along with execution examples and user interactions.java code

package Calculator;

import java.util.Scanner;

public class Task1Calculator {


	public static void main(String[] args) {

		Scanner sca=new Scanner(System.in);
		int n1,n2;

		boolean flag=true;

		while(flag) {


			System.out.println("1.ADD\n2.Substraction\n3.Multiply\n4.Divide\n5.Exponentiation\n6.Quit");
			System.out.println("Select Operation : ");
			int choice=sca.nextInt();

			if(choice==6) {
	            	System.out.println("Thank you!!,Calculator is Exit!!");
	            	break;
	            }

			int result=0;
			System.out.println("enter first Number : ");
			n1=sca.nextInt();
			System.out.println("enter Second Number : ");
			n2=sca.nextInt();

			switch(choice) {


			case 1:
				         result = n1 + n2;
				         break;
			case 2:
				         result = n1 - n2;
				         break;
			case 3:
			           	 result = n1 * n2;
				         break;
			case 4:
				         if (n2 == 0) {
					     System.out.println("Error!!,We can't devide With '0' ");
				         } else
					 result = n1 / n2;
				         break;
			case 5:
				        result=(int)Math.pow(n1, n2);
				        break;

		       default:
		    	                System.out.println("In-valied Choice!!,choice Correct One!!");
		    	                break;

			}

			System.out.println("Result is : "+result);
			System.out.println("-------------------------");

		}
		sca.close();
	}



}

Documentation Overview: 

The Calculator program is a Java application that allows users to perform basic arithmetic operations such as addition, subtraction, multiplication, division, and exponentiation. It provides a menu-driven interface where users can select the desired operation, input two numbers, and obtain the result.

Features: Menu-driven Interface: Users are presented with a menu of operation choices, and they can select an option based on their requirement.

Arithmetic Operations: The calculator supports addition, subtraction, multiplication, division, and exponentiation.

Looping Structure: The program utilizes a while loop to continuously prompt the user for input until they choose to quit.

Error Handling: If the user enters an invalid operator choice, the program displays an error message and prompts the user to choose again.

How it Works:

1.Initialization:

The program starts by importing the Scanner class to handle user input.
It declares variables n1 and n2 to store the user's input for two numbers.
It also initializes a boolean variable flag to control the main loop.

2.Main Loop:
The program enters a while loop controlled by the flag variable.
Inside the loop, the user is presented with a menu of operations:

1.Addition
2.Subtraction
3.Multiplication
4.Division
5.Exponentiation
6.Quit

The user is prompted to select an operation by entering a corresponding number.

3.Operation Selection:
The program reads the user's choice using the nextInt() method of the Scanner object.
If the user selects option 6 (Quit), the program prints a farewell message and exits the loop.
Otherwise, the program proceeds to prompt the user for two numbers.

4.Performing Operations:
Depending on the user's choice, the program performs the selected arithmetic operation on the two input numbers.
It uses a switch-case statement to determine the operation based on the user's choice.
The result of the operation is stored in the result variable.

5.Error Handling:
If the user selects division (option 4) and the second number is zero, the program prints an error message indicating that division by zero is not allowed.
Output:

After performing the operation, the program prints the result to the console.
Additionally, it prints a line of dashes to separate each calculation.

6.Loop Continuation:
The loop continues until the user chooses to quit (option 6).
Resource Cleanup:
Finally, the program closes the Scanner object to release system resources.

Execution Example:
User Interaction:
 The user is presented with a menu of operation choices.
 User select an operation by entering the corresponding number. 
 user enter two numbers as inputs for the selected operation. 
 The result of the operation is displayed.
 User can choose to perform another calculation or exit the program.
 
Conclusion: 
The Simple Calculator program provides a basic yet functional tool for performing arithmetic calculations.
Its user-friendly interface and error handling make it suitable for simple mathematical tasks. 
The modular structure of the code allows for easy maintenance and future enhancements.
