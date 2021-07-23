# CompSciCaptsone

## C++ Grading Program
 
```
#include<iostream>
using namespace std;
int main()
                   {

        /*Create placeholder for 5 assignments and set initial average to 0*/
        int grade[5], i;
        float sum=0,avg;


        /*Ask for grades on the 5 assignments*/
        cout<<"\n Enter Student's grades for the 5 assignments: \n -----------------------------------------------";

        /*List name of assignments*/
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

        for(i=0;i<5;i++)
        {
                sum=sum+grade[i];
        }

        /*Find sum of assignments and then calculate average. Print out letter grade based on average.*/
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
