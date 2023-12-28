#include<iostream>
using namespace std;
int main()
{
    cout<<"Hello World"<<endl;

    return 0;
}

#include<iostream>
#include<conio.h>
using namespace std;

int main()
{
    double farn,cels;
    cout<<"Enter celius : \n";
    cin>>cels;

    farn = 1.8* cels+ 32;

    cout<<"Fahrenheit = "<<farn;

    getch();

}

toupper() && tolower
#include<iostream>
using namespace std;
int main()
{
    char ch;

    cout<<"Enter any letter : ";
    cin>>ch;

    ch = tolower(ch);
    if (ch=='a'||ch=='e'||ch=='i'||ch=='o'||ch=='u') {
        cout<<"Vowel";
    }
    else {
    cout<<"Consonant";
    }

    return 0;

}

//Leap Year program
#include<iostream>
using namespace std;

int main() {
   int year;
   cout << "Enter any year: ";
   cin >> year;

   if ((year % 4 == 0 && year % 100 != 0) || (year % 400 == 0)) {
       cout << "Leap Year";
   }
   else {
       cout << "Not Leap Year";
   }

   return 0;
}

// conditional operator / Ternary Operator

#include<iostream>
using namespace std;

int main() {
   int num1,num2;
   num1=90;
   num2=34;

   int max =(num1>num2)?num1:num2;
   cout<<max;
   return 0;
}
// conditional operator / Ternary Operator
#include<iostream>
using namespace std;

int main() {
   int num;
   cout<<"Enter any integer : ";
   cin>>num;

   (num%2==0)?cout<<num<<" is even " :cout<<num<<" is odd";

   return 0;
}

//while loop
#include<iostream>
using namespace std;

int main(){
    int i=1;//initalization
    while(i<=100)//condition check
    {
        cout<<i<<endl;
        i++;//increment
    }
    cout<<"End of while loop";
   return 0;
}

//do while
#include<iostream>
using namespace std;

int main(){
    int i=0;//initalization
    do{
        cout<<i<<endl;
        i++;//increment
    }
    while(i<=100);

    cout<<"End of while loop";
   return 0;
}

//Multiplication table
#include<iostream>
using namespace std;

int main(){

    int num;
        cout<<"Enter any integer number : ";
        cin>>num;

        for(int i=1;i<=10;i++)
        {
            cout<<num<< " X "<< " = "<<(num*i)<<endl;
        }

    cout<<" The  End ";
   return 0;
}

#include<iostream>
using namespace std;
int main()
{
    int sum=0,n;
    cout<<"Enter the last number : ";
    cin>>n;
    cout << "The sum of the sequence 1+2+3+..+" << n << " is: "<<endl;

     for(int i=1;i<=n;i=i+1)
    {
        sum=sum+i;
    }
    cout<<sum;
    return 0;
}
//array
#include<iostream>
#include<conio.h>
using namespace std;
int main()
{
    int num[5]={1,12,3,3,4};
    for(int i=0;i<5;i++)
    {
        cout<<num[i]<< " ";
    }
    getch();
}
//#include<iostream>
#include<conio.h>
using namespace std;
int main()
{
    int num[5];
    for(int i=0;i<5;i++)
    {
        cout<<"Marks for student " <<i+1 <<"=";
        cin>>num[i];
    }
    cout<<"Number are ";
    for(int i=0;i<5;i++)
    {
        cout<<num[i]<< " ";
    }
    getch();
}

//maximum &minimum
#include<iostream>
#include<conio.h>
using namespace std;
int main()
{
    int n,sum=0;
    cout<<"Enter Number of student : ";
    cin>>n;
    int student[n];
    //input
    for(int i=0;i<n;i++)
    {
        cout<<"Marks for student : "<< i+1<<"=";
        cin>>student [i];
        sum =sum + student[i];
    }
    cout<<"Total marks : "<<sum<<endl;
    float avg=(float)sum/n;
    cout<<"Average "<<avg<<endl;

    int max=student[0];
    int min=student[0];

    for(int i=1;i<n;i++)
    {
        if(max<student[i])
        {
            max=student[i];
        }
         if(min>student[i])
        {
            min=student[i];
        }
    }
    cout<<"Maximum marks = "<<max<<endl;
    cout<<"Minimum marks = "<<min;

    getch();
}
//matrix
#include<iostream>
#include<conio.h>
using namespace std;

int main() {
    int a[2][2];

    cout<<"Enter the elements : "<<endl;
    // Input values into the array
    for(int r=0; r<2; r++)
    {
        for(int c=0; c<2; c++)
        {
            cout << "A[" <<r<<"] [" <<c<< "] = ";
            cin >> a[r][c];
        }
    }

    // Output the array
    cout<<"A Matrix = "<<endl;
    for(int r=0; r<2; r++)
    {
        for(int c=0; c<2; c++)
        {
            cout << a[r][c] << " ";
        }
        cout << endl;
    }

    getch();
    return 0;
}

//simple array
#include<iostream>
#include<conio.h>
using namespace std;

int main() {
    int i, j;
    int A[3][3],B[3][3];

    cout<<"Enter elements for A Matrix : "<<endl;
    // Input values into the array
    for(i = 0; i < 3; i++)
    {
        for(j = 0; j < 3; j++)
        {
            cout<< "A ["<< i<<" ][" << j << "] = ";
            cin>> A[i][j]; // Add & before A[i][j]
        }
        cout<<endl;
    }

        for(i = 0; i < 3; i++)
    {
        for(j = 0; j < 3; j++)
        {
            cout<< "B ["<< i<<" ][" << j << "] = ";
            cin>> B[i][j]; // Add & before A[i][j]
        }
        cout<<endl;
    }

    // Output the array
    cout << "A = ";
    for(i = 0; i < 3; i++)
    {
        cout << "\t";
        for(j = 0; j < 3; j++) {
            cout << A[i][j] << " "; // Print a space after each element
        }
        cout << endl; // Add a newline after each row
    }

   cout << "B = ";
    for(i = 0; i < 3; i++)
    {
        cout << "\t";
        for(j = 0; j < 3; j++) {
            cout << B[i][j] << " "; // Print a space after each element
        }
        cout << endl; // Add a newline after each row
    }

    getch();
    return 0;
}

//Sum of matrix
#include<iostream>
#include<conio.h>
using namespace std;

int main() {
    int i, j;
    int A[3][3],B[3][3],c[3][3];

    cout<<"Enter elements for A Matrix : "<<endl;
    // Input values into the array
    for(i = 0; i < 3; i++)
    {
        for(j = 0; j < 3; j++)
        {
            cout<< "A ["<< i<<" ][" << j << "] = ";
            cin>> A[i][j]; // Add & before A[i][j]
        }
        cout<<endl;
    }

        for(i = 0; i < 3; i++)
    {
        for(j = 0; j < 3; j++)
        {
            cout<< "B ["<< i<<" ][" << j << "] = ";
            cin>> B[i][j]; // Add & before A[i][j]
        }
        cout<<endl;
    }
//calculate sum
    for(i=0;i<3;i++)
    {
        for(j=0;j<3;j++)
        {
            c[i][j]=A[i][j]+B[i][j];
        }
    }
    // Output the array
    cout << "A = ";
    for(i = 0; i < 3; i++)
    {
        cout << "\t";
        for(j = 0; j < 3; j++) {
            cout << A[i][j] << " "; // Print a space after each element
        }
        cout << endl; // Add a newline after each row
    }

   cout << "B = ";
    for(i = 0; i < 3; i++)
    {
        cout << "\t";
        for(j = 0; j < 3; j++) {
            cout << B[i][j] << " "; // Print a space after each element
        }
        cout << endl; // Add a newline after each row
    }

    cout<<"Sum=";
     for(i = 0; i < 3; i++)
    {
        cout << "\t";
        for(j = 0; j < 3; j++) {
            cout << c[i][j] << " ";
        }
        cout << endl;
    }


    getch();
    return 0;
}
//subtraticon

#include<iostream>
#include<conio.h>
using namespace std;

int main() {
    int i, j;
    int A[3][3],B[3][3],c[3][3];

    cout<<"Enter elements for A Matrix : "<<endl;
    // Input values into the array
    for(i = 0; i < 3; i++)
    {
        for(j = 0; j < 3; j++)
        {
            cout<< "A ["<< i<<" ][" << j << "] = ";
            cin>> A[i][j]; // Add & before A[i][j]
        }
        cout<<endl;
    }

        for(i = 0; i < 3; i++)
    {
        for(j = 0; j < 3; j++)
        {
            cout<< "B ["<< i<<" ][" << j << "] = ";
            cin>> B[i][j]; // Add & before A[i][j]
        }
        cout<<endl;
    }
//calculate sum
    for(i=0;i<3;i++)
    {
        for(j=0;j<3;j++)
        {
            c[i][j]=A[i][j]+B[i][j];
        }
    }
    // Output the array
    cout << "A = ";
    for(i = 0; i < 3; i++)
    {
        cout << "\t";
        for(j = 0; j < 3; j++) {
            cout << A[i][j] << " "; // Print a space after each element
        }
        cout << endl; // Add a newline after each row
    }

   cout << "B = ";
    for(i = 0; i < 3; i++)
    {
        cout << "\t";
        for(j = 0; j < 3; j++) {
            cout << B[i][j] << " "; // Print a space after each element
        }
        cout << endl; // Add a newline after each row
    }

    cout<<"Minus=";
     for(i = 0; i < 3; i++)
    {
        cout << "\t";
        for(j = 0; j < 3; j++) {
            cout << c[i][j] << " ";
        }
        cout << endl;
    }


    getch();
    return 0;
}

