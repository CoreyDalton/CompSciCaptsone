# CompSciCaptsone

<h1>Software Design & Engineering</h1>

## Narrative

### Briefly describe the artifact. What is it? When was it created?

The original artifact is a C++ program that is used to calculate the average score and letter grade for a student. I created this program when I was enrolled in a programming course at another college that I attended. 
   
### Justify the inclusion of the artifact in your ePortfolio. Why did you select this item? What specific components of the artifact showcase your skills and abilities in # software development? How was the artifact improved?

The reason that I selected this item was because I felt it would be a good example of my ability and understanding of multiple languages. As per the rubric, one of the possible options was to consider transferring a project into a different language, and that is just what I did with this. I wouldn’t necessarily say that the artifact was improved in terms of ability, but it has been transformed to something that could be implemented in a larger Java project, rather than solely for C++. 

## Original C++ Grading Program
 
```C++
/*
 * Grading.cpp
 */


#include<iostream>
using namespace std;
int main()
                   {

        //Create placeholder for 5 assignments and set initial average to 0
        int grade[5], i;
        float sum=0,avg;


        //Ask for grades on the 5 assignments
        cout<<"\n Enter Student's grades for the 5 assignments: \n -----------------------------------------------";

        //Output assignment designations, one-at-a-time, and request grade input for each
        cout<<"\n Assignment 1: ";
        cin>>grade[0];
        cout<<"\n Assignment 2: ";
        cin>>grade[1];
        cout<<"\n Assignment 3: ";
        cin>>grade[2];
        cout<<"\n Assignment 4: ";
        cin>>grade[3];
        cout<<"\n Assignment 5: ";
        cin>>grade[4];

        //Find sum of assignments
        for(i=0;i<5;i++)
        {
                sum=sum+grade[i];
        }

        //Calculate average. Print out letter grade based on average.
        cout<<"-----------------------------------------------\n Sum of all graded assignments = "<<sum;
        avg=sum/5;
        cout<<"\n Average: "<<avg;
        cout<<"\n Final Calculated Grade: ";

        if(avg>89)
        {
                cout<<"A";
        }
        else if(avg>79 && avg<=89)
        {
                cout<<"B";
        }
        else if(avg>69 && avg<=79)
        {
                cout<<"C";
        }
        else if(avg>59 && avg<=69)
        {
                cout<<"D";
        }
        else
        {
                cout<<"F";
        }
        return 0;
}

```
## Enahnced Java Grading Program

```Java
import java.util.Scanner;

public class JavaGrading
{
    public static void main(String args[])
    {
    	// Create placeholder for 5 assignments, set initial sum of grades to 0, declare avg variable & keyboard scanner
        int grades[] = new int[5];
        int i;
        float sum=0, avg;
        Scanner scanner = new Scanner(System.in);
		
        //Output assignment designations, one-at-a-time, and request grade input for each
        System.out.print("Enter Student's grades for the 5 assignments:");
        for(i=0; i<5; i++) { 
           System.out.print("\nAssignment " + (i+1) + ": ");
           grades[i] = scanner.nextInt();
           sum = sum + grades[i];
        }
        scanner.close();
        //Calculate average score of the 5 assignments and determine letter grade for student
        avg = sum/5;
        System.out.print("-----------------------------------------------\nSum of all graded assignments: " + sum);
        System.out.print("\nAverage: " + avg);
        System.out.print("\nFinal Calculated Grade: ");
        if(avg>89)
        {
            System.out.print("A");
        }
        else if(avg>79 && avg<=89)
        {
           System.out.print("B");
        } 
        else if(avg>69 && avg<=79)
        {
            System.out.print("C");
        }
        else if(avg>59 && avg<=69)
        {
            System.out.print("D");
        }
        else
        {
            System.out.print("F");
        }
    }
}

```
### Reflect on the process of enhancing and/or modifying the artifact. What did you learn as you were creating it and improving it? What challenges did you face?

Throughout the process of transferring this C++ program into Java, I learned that, at least at a base level, the two languages are fairly similar and having a basic understanding of both proved to be very useful in the translation process. The biggest challenge that I faced was going back to coding in Java and remembering how the language works in comparison to C++. It had been some time since I had done any coding in Java, so it took a bit longer than it would have if I had been practicing in the language.
