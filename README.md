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
//mutiplication
#include<iostream>
#include<conio.h>
using namespace std;
int main()
{
    int a[10][10],b[10][10],r[10][10],sum=0,r1,r2,c1,c2,i,j,k;

    cout<<"Enter  row and col for first matrix: ";
    cin>>r1>>c1;

    cout<<"Enter  row and col for 2nd matrix: ";
    cin>>r2>>c2;

    while(c1!=r2)
    {
        cout<<"Error !! colum of first matrix not equal to row of second matrix"<<endl;

        cout<<"Enter row and col for first matrix: ";
        cin>>r1>>c1;
        cout<<"Enter  row and col for 2nd matrix: ";
        cin>>r2>>c2;
    }
    cout<<"Enter elements for first matrix\n";
     for (i = 0; i < r1; i++)
    {
        for (j = 0; j < c1; j++)
            {
            cout << "a [" << i << "] [" << j << "] = ";
            cin >> a[i][j];
            }
    }

    cout << "\nEnter elements for second matrix\n";
    for (i = 0; i < r2; i++)
    {

        for (j = 0; j < c2; j++)
            {
            cout << "b[" << i << "] [" << j << "] = ";
            cin >> b[i][j];
            }
    }
        // Multiplication
    for (i = 0; i < r1; i++)
        {
        for (j = 0; j < c2; j++)
        {
            for (k = 0; k < c1; k++)
            {
                sum = sum + a[i][k] * b[k][j];
            }
            r[i][j] = sum;
            sum = 0;
        }
    }
    cout << "\n\nFirst Matrix \n";
    for (i = 0; i < r1; i++) {
        for (j = 0; j < c1; j++)
            cout << a[i][j] << " ";
        cout << endl;
    }

    cout << "\n\nSecond Matrix \n";
    for (i = 0; i < r2; i++) {
        for (j = 0; j < c2; j++)
            cout << b[i][j] << " ";
        cout << endl;
    }

    cout << "\n\nResult Matrix \n";
    for (i = 0; i < r1; i++) {
        for (j = 0; j < c2; j++)
            cout << r[i][j] << " ";
        cout << endl;
    }

    getch();
}

//pointer
#include<iostream>
#include<conio.h>
using namespace std;
int main()
{
    int x=5;
    int *p;
    p=&x;//x er address rakci p pointer a

    cout<< x <<endl;
    cout<< &x <<endl;//adress
    cout<< p <<endl;
    cout<< *p <<endl;//p er value
    
    getch();

}
 Adding 2 Numbers Using Pointer
#include<iostream>
#include<conio.h>
using namespace std;
int main()
{
    int x1=5;
    int x2=15;
    int *p1,*p2;

    p1=&x1;
    p2=&x2;

    int sum=*p1+*p2;
    cout<<sum;

    getch();

}
//declaring multiple function
#include<iostream>
#include<conio.h>
using namespace std;
void addition(int a,int b)
{
    int sum = a+b;
    cout<<sum<<endl;
}
int main()
{
    addition(20,20);
    getch();
}




